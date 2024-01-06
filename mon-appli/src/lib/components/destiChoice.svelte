<script lang="ts">
	let selectedDestinations: string[] = [];

	const destinations = [
		{ category: 'Calvados', stays: ['Séjour 1', 'Séjour 2', 'Séjour 3', 'Séjour 4'] }
		// Ajoutez d'autres catégories et séjours au besoin
	];

	function handleCheckboxChange(event: Event, destination: string, category: string) {
		if (event.target instanceof HTMLInputElement && event.target.checked) {
			selectedDestinations = [...selectedDestinations, `${category} - ${destination}`];
		} else {
			selectedDestinations = selectedDestinations.filter(
				(dest) => dest !== `${category} - ${destination}`
			);
		}
	}

	function handleSubmit(category: string) {
		// Ajoutez ici la logique pour traiter les séjours sélectionnés dans la catégorie spécifiée
		console.log(`Séjours sélectionnés pour ${category}:`, selectedDestinations);
	}
</script>

{#if selectedDestinations.length > 0}
	<div>
		<h2>Destinations sélectionnées :</h2>
		<ul>
			{#each selectedDestinations as destination}
				<li>{destination}</li>
			{/each}
		</ul>
	</div>
{/if}

{#each destinations as { category, stays }}
	<div class="destination-card">
		<h3>Destination</h3>
		<div>
			<strong>{category}</strong>
		</div>
		{#each stays as stay}
			<label>
				<input type="checkbox" on:change={(e) => handleCheckboxChange(e, stay, category)} />
				{stay}
			</label>
		{/each}
		<button on:click={() => handleSubmit(category)}>Valider</button>
	</div>
{/each}

<style>
	.destination-card {
		border: 1px solid #ccc;
		padding: 10px;
		margin: 10px;
		border-radius: 5px;
		position: relative; /* Pour permettre un positionnement absolu à l'intérieur */
	}

	label {
		display: block; /* Chaque case à cocher sur une nouvelle ligne */
	}

	button {
		background-color: #ff4380;
		color: white;
		padding: 10px;
		border: none;
		border-radius: 5px;
		width: 100%; /* Prend toute la largeur de la carte */
		position: absolute;
		bottom: 0; /* Aligné en bas de la carte */
		left: 0; /* Aligné à gauche de la carte */
	}
</style>

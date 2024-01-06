<script lang="ts">
	let showDestiChoice = false;

	function handleButtonClick() {
		showDestiChoice = true;
	}
</script>

<form>
	<!-- Vous pouvez ajouter vos champs de formulaire ici -->
	<h1>Rechercher votre séjour</h1>
	<form on:submit|preventDefault={handleButtonClick}></form>
	<p><input type="submit" value="Choix du séjour   ->" /></p>
	<p>
		<input type="submit" value="Date de séjour / Arrivée - Départ ->" />
	</p>
	<p><input type="submit" value="Hébergement et participant ->" /></p>
	<p><input type="submit" value="Location de vélo ->" /></p>
	<p><input type="submit" value="Reservation de brunch ou planche Apéro ->" /></p>
</form>

<style>
	input[type='submit'] {
		border-radius: 10px;
		box-shadow: 0 3px 3px black;
		transition: background-color 0.5s ease;
		width: 100%;
		height: 80px;
		padding: 10px;
	}

	input[type='submit']:hover {
		background-color: rgb(147, 162, 147);
	}
</style>

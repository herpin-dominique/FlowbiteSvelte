<script lang="ts">
	import SelectTrip from '$lib/components/SelectTrip.svelte';
	import FloChecbox from '$lib/components/FloChecbox.svelte';
	import Form from '$lib/components/Form.svelte';
	import { DateInput } from 'date-picker-svelte';

	let date = new Date();
</script>

<section>
	<div class="searchEngine-mobile">
		<div class="searchForm-block-staySelectContainer">
			<span class="icon-location"></span>
			<span id="searchToggler-sejours">Choisir un séjour </span>
		</div>

		<div class="searchForm-block-dateParticipants">
			<span class="searchToggler-participants">
				<i class="icon-cottage"></i>
				<span id="searchToggler-nbCottage">1 </span>
				<i class="icon-participant"></i>
				<span id="searchToggler-nbParticipant"> 2</span>
				<span class="searchToggler-date">
					<i class="icon-calendar"></i>
					<span id="searchToggler-dates"> Dates de séjour</span>
				</span>
			</span>
		</div>
		<button class="home search label nos sticky">Rechercher</button>
	</div>
</section>
<section>
	<SelectTrip />
</section>
<section>
	<FloChecbox />
	<Form />
</section>
<DateInput bind:value={date} />

<style>
	@import url('https://i.icomoon.io/public/temp/6f841c1106/UntitledProject/style.css');

	.icon-cottage:before {
		content: '\e900';
	}
	.icon-participant:before {
		content: '\e972';
	}
	.icon-location:before {
		content: '\e948';
	}
	.icon-calendar:before {
		content: '\e901';
	}
	.searchEngine-mobile {
		position: relative;
		margin-top: 20vh;
		border: 2px solid;
		border-radius: 20px 20px 0 0;
		width: 70%;
		height: 100px;
	}

	:global(body) {
		display: flex;
		justify-content: center;
	}
	.searchForm-block-staySelectContainer {
		padding: 10px;
		border-bottom: 2px solid #f4f5f5;
		width: 90%;
		margin-left: 10px;
	}
	.searchForm-block-dateParticipants {
		padding: 10px;
		margin-left: 10px;
	}
	#searchToggler-nbParticipant {
		border-right: 2px solid #f4f5f5;
		padding-right: 5px;
	}
	/* Style pour le bouton "Rechercher" */
	.home.search.label.nos.sticky {
		margin-top: 9px; /* Ajoutez une marge en haut pour séparer le bouton des éléments ci-dessus */
		padding: 10px;
		background-color: #ff4380; /* Couleur de fond du bouton */
		color: #fff; /* Couleur du texte du bouton */
		border: 2px solid #000;
		border-bottom-left-radius: 15px;
		border-bottom-right-radius: 15px; /* Ajoutez une bordure arrondie */
		cursor: pointer;
		width: 100%;
	}
	@media (max-width: 480px) {
		section {
			display: flex;
			flex-direction: column;
		}
	}
</style>

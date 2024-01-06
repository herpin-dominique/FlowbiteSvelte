<script>
	import { Checkbox } from 'flowbite-svelte';
</script>

<div class="destination-header">
	<h1>DESTINATION</h1>
</div>

<div class="destination-container">
	<p class="mb-4 font-semibold text-gray-900 dark:text-white">Destinations</p>
	<ul
		class="w-48 divide-y divide-gray-200 rounded-lg border border-gray-200 bg-white dark:divide-gray-600 dark:border-gray-600 dark:bg-gray-800"
	>
		<li><Checkbox class="p-3">SEJOUR DE CAEN A PONT D'OUILLY</Checkbox></li>
		<li><Checkbox class="p-3">DE CAEN SAINT AUBIN SUR MER</Checkbox></li>
		<li><Checkbox class="p-3">DE CAEN A VILLERS SUR MER</Checkbox></li>
		<li><Checkbox class="p-3">DE PONT D'OUILLY A VILLERS SUR MER</Checkbox></li>
	</ul>

	<button class="full-width-button">Valider</button>
</div>

<style>
	.destination-header {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		background-color: #fff;
		padding: 10px;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
		z-index: 100;
	}

	.destination-container {
		margin-top: 40px;
	}
	.full-width-button {
		width: 100%;
		background-color: #ff4380;
		color: white;
		padding: 10px;
		border: none;
		border-radius: 5px;
		margin-top: 10px; /* Ajustez selon votre espacement souhaité */
	}
</style>

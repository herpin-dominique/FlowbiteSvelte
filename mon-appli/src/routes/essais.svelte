<!-- <script lang="ts">
	// import { Card, Button, Toggle, Label, Input, Checkbox } from 'flowbite-svelte';
	// import { ArrowRightOutline } from 'flowbite-svelte-icons';
	// import { CheckCircleSolid } from 'flowbite-svelte-icons';
	// let vCard = false;
	// import { navigate } from '@sveltekit';
	import { onMount } from 'svelte';

	let stay = '';
	let bike = '';
	let people = '';
	let date = '';

	const handleSubmit = () => {
		const query = `stay=${stay}&bike=${bike}&people=${people}&date=${date}`;
		navigate(`/search?${query}`);
	};

	onMount(() => {
		// Initialize Flowbite components
		window.FlowBite.init();
	});
</script>

<div class="flowbite">
	<div class="container">
		<form on:submit|preventDefault={handleSubmit}>
			<div class="form-group">
				<label for="stay">Choisir un séjour:</label>
				<select id="stay" bind:value={stay} class="form-control">
					<option value="">--Choisir un séjour--</option>
					<option value="sejour1">Séjour 1</option>
					<option value="sejour2">Séjour 2</option>
					<option value="sejour3">Séjour 3</option>
				</select>
			</div>

			<div class="form-group">
				<label for="bike">Choisir un vélo:</label>
				<select id="bike" bind:value={bike} class="form-control">
					<option value="">--Choisir un vélo--</option>
					<option value="velo1">Vélo 1</option>
					<option value="velo2">Vélo 2</option>
					<option value="velo3">Vélo 3</option>
				</select>
			</div>

			<div class="form-group">
				<label for="people">Choisir un nombre de personnes:</label>
				<select id="people" bind:value={people} class="form-control">
					<option value="">--Choisir un nombre de personnes--</option>
					<option value="senior">Senior</option>
					<option value="enfant">Enfant</option>
					<option value="adultes">Adultes</option>
				</select>
			</div>

			<div class="form-group">
				<label for="date">Choisir une date de réservation:</label>
				<input type="date" id="date" bind:value={date} class="form-control" />
			</div>

			<button type="submit" class="btn btn-primary">Rechercher</button>
			<button type="reset" class="btn btn-secondary">Réinitialiser</button>
		</form>
	</div>
</div> -->

<!-- <div class="grid-container">
	<Card img="\src\Images\IMG_1188.JPG" reverse={vCard} class="mb-4">
		<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
			Belle carte avec une écriture en gras 2023
		</h5>
		<p class="mb-3 font-normal leading-tight text-gray-700 dark:text-gray-400">
			Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
			chronological order.
		</p>
		<Button>
			En savoir plus <ArrowRightOutline class="ms-2 h-3.5 w-3.5 text-white" />
		</Button>
	</Card>
	<Toggle bind:checked={vCard} class="italic dark:text-gray-500">Reverse</Toggle>
</div>

<div class="grid-container">
	<Card img="\src\Images\IMG_1188.JPG" reverse={vCard} class="mb-4">
		<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
			Belle carte avec une écriture en gras 2023
		</h5>
		<p class="mb-3 font-normal leading-tight text-gray-700 dark:text-gray-400">
			Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
			chronological order.
		</p>
		<Button>
			En savoir plus <ArrowRightOutline class="ms-2 h-3.5 w-3.5 text-white" />
		</Button>
	</Card>
	<Toggle bind:checked={vCard} class="italic dark:text-gray-500">Reverse</Toggle>
</div>

<div class="grid-container">
	<Card img="\src\Images\IMG_1188.JPG" reverse={vCard} class="mb-4">
		<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
			Belle carte avec une écriture en gras 2023
		</h5>
		<p class="mb-3 font-normal leading-tight text-gray-700 dark:text-gray-400">
			Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
			chronological order.
		</p>
		<Button>
			En savoir plus <ArrowRightOutline class="ms-2 h-3.5 w-3.5 text-white" />
		</Button>
	</Card>
	<Toggle bind:checked={vCard} class="italic dark:text-gray-500">Reverse</Toggle>
</div>
<Card class="w-full max-w-md">
	<form class="flex flex-col space-y-6" action="/">
		<h3 class="text-xl font-medium text-gray-900 dark:text-white">Sign in to our platform</h3>
		<Label class="space-y-2">
			<span>Email</span>
			<Input type="email" name="email" placeholder="name@company.com" required />
		</Label>
		<Label class="space-y-2">
			<span>Your password</span>
			<Input type="password" name="password" placeholder="•••••" required />
		</Label>
		<div class="flex items-start">
			<Checkbox>Remember me</Checkbox>
			<a href="/" class="ms-auto text-sm text-primary-700 hover:underline dark:text-primary-500">
				Lost password?
			</a>
		</div>
		<Button type="submit" class="w-full">Login to your account</Button>
		<div class="text-sm font-medium text-gray-500 dark:text-gray-300">
			Not registered? <a href="/" class="text-primary-700 hover:underline dark:text-primary-500">
				Create account
			</a>
		</div>
	</form> -->
<!-- <Card padding="xl">
	<h5 class="mb-4 text-xl font-medium text-gray-500 dark:text-gray-400">Forfait Week-end</h5>
	<div class="flex items-baseline text-gray-900 dark:text-white">
		<span class="text-3xl font-semibold"></span>
		<span class="text-5xl font-extrabold tracking-tight">250 EUROS</span>
		<span class="ms-1 text-xl font-normal text-gray-500 dark:text-gray-400">/PERSONNES</span>
	</div> -->
<!-- List -->
<!-- <ul class="my-7 space-y-4">
		<li class="flex space-x-2 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-primary-600 dark:text-primary-500" />
			<span class="text-base font-normal leading-tight text-gray-500 dark:text-gray-400">
				2 PERS.
			</span>
		</li>
		<li class="flex space-x-2 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-primary-600 dark:text-primary-500" />
			<span class="text-base font-normal leading-tight text-gray-500 dark:text-gray-400">
				2 Vélos à assistance electrique
			</span>
		</li>
		<li class="flex space-x-2 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-primary-600 dark:text-primary-500" />
			<span class="text-base font-normal leading-tight text-gray-500 dark:text-gray-400">
				1 Logement insolite
			</span>
		</li>
		<li class="flex space-x-2 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-primary-600 dark:text-primary-500" />
			<span class="text-base font-normal leading-tight text-gray-500 dark:text-gray-400">
				1 plateau apéro Normand
			</span>
		</li>

		<li class="flex space-x-2 line-through decoration-gray-500 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-gray-400 dark:text-gray-500" />
			<span class="text-base font-normal leading-tight text-gray-500">1 parcours détaillé</span>
		</li>
		<li class="flex space-x-2 line-through decoration-gray-500 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-gray-400 dark:text-gray-500" />
			<span class="text-base font-normal leading-tight text-gray-500"
				>1 Documentation complète de la région</span
			>
		</li>
		<li class="flex space-x-2 line-through decoration-gray-500 rtl:space-x-reverse">
			<CheckCircleSolid class="h-4 w-4 text-gray-400 dark:text-gray-500" />
			<span class="text-base font-normal leading-tight text-gray-500"
				>24×7 phone & email support</span
			>
		</li>
	</ul> -->
<!-- <Button class="w-full">Choisir ce pack</Button> -->

<!-- </Card> -->

<!-- </Card> -->

<!-- <style>
	.grid-container {
		display: flex;
		grid-template-columns: repeat(3, 1fr);
		justify-content: center;
		margin-bottom: 20px; /* Ajoutez une marge entre les rangées de cartes si nécessaire */
	}
</style> -->
<!-- <script>
</script>

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
</div> -->

<script>
	import { Datepicker } from 'flowbite-svelte';
	let name = '';
	let email = '';
	let date = '';
	let time = '';
	let people = '';

	function handleSubmit() {
		// Ajoutez ici le code pour traiter le formulaire
	}
</script>

<head>
	...
	<link rel="stylesheet" href="/node_modules/flowbite/dist/flowbite.min.css" />
	<script src="/node_modules/flowbite/dist/flowbite.bundle.js"></script>
</head>
<form on:submit|preventDefault={handleSubmit}>
	<div class="mb-3">
		<label for="name" class="form-label">Nom</label>
		<input type="text" id="name" class="form-control" bind:value={name} required />
	</div>
	<div class="mb-3">
		<label for="email" class="form-label">Email</label>
		<input type="email" id="email" class="form-control" bind:value={email} required />
	</div>
	<div class="mb-3">
		<label for="date" class="form-label">Date</label>
		<Datepicker id="date" bind:value={date} required />
	</div>
	<div class="mb-3">
		<label for="time" class="form-label">Heure</label>
		<input type="time" id="time" class="form-control" bind:value={time} required />
	</div>
	<div class="mb-3">
		<label for="people" class="form-label">Nombre de personnes</label>
		<input type="number" id="people" class="form-control" bind:value={people} min="1" required />
	</div>
</form>

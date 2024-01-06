<script lang="ts">
	import { goto } from '$app/navigation';
	function redirectToCalendrier() {
		goto('/src/lib/components/Calendrier.svelte');
	}
	function redirectToReservation() {
		goto('/src/lib/components/ReservationForm.svelte');
	}
	function redirectToChoixSejour() {
		goto('/src/lib/components/ChoixSejour.svelte');
	}
</script>

<form>
	<button type="button" on:click={redirectToCalendrier}>go to calendrier</button>
	<button type="button" on:click={redirectToReservation}>go to selection-personnes</button>
	<button type="button" on:click={redirectToChoixSejour}>go to choix sejour</button>
</form>

<style>
	button {
		width: 100%;
		padding: 10px;
		margin: 10px;
		background-color: #ff4380;
	}
</style>

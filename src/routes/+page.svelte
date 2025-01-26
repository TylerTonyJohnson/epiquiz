<script>
	import { goto } from '$app/navigation';
	import Card from '$lib/Card.svelte';

	function handleClick() {
		goto('/Question1');
	}
</script>

<Card>
	<h1>Are you ready for your quiz?</h1>
	<button onclick={handleClick}>Let's go!</button>
</Card>

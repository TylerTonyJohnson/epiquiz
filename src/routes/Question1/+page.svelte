<script lang="ts">
	import { goto } from '$app/navigation';
	import Card from '$lib/Card.svelte';
	import type { PageData } from './$types';

	let { data }: { data: PageData } = $props();

	let answer = 'Paris';
	let input = $state('');

	function handleClick() {
		if (input === answer) {
			goto('/Question2');
		}
	}
</script>

<div class="frame">
	<Card>
		<h1>Question 1</h1>
		<p>What is the capital of France?</p>
		<textarea bind:value={input}></textarea>
		<button onclick={handleClick} disabled={input !== answer}>Continue</button>
	</Card>
</div>

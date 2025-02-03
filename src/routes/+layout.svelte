<script lang="ts">
	import type { Snippet } from 'svelte';
	import type { LayoutData } from './$types';

	let { data, children }: { data: LayoutData; children: Snippet } = $props();

	import '../app.css';
</script>

<div class="frame">
	{@render children()}
</div>

<style>
	.frame {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: start;
		/* width: 100%; */
		min-height: 100vh;
		padding: 4rem;
		gap: 2rem;
		/* background-color: chocolate; */
		/* background-size: 100vw 100vh; */

		background-image: linear-gradient(62deg, #fbab7e 0%, #f7ce68 100%);

		color: white;
	}
</style>

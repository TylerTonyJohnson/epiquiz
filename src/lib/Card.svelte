<script>
	let { children } = $props();
</script>

<div class="frame">
	{@render children()}
</div>

<style>
	.frame {
		min-width: 40rem;
		min-height: 10rem;
		border: solid 2px white;
		display: flex;
		flex-direction: column;
		place-content: center;
		padding: 5rem;
		gap: 2.5rem;
		border-radius: 2rem;
		/* background-color: #0004; */
		background-image: linear-gradient(to bottom, #0003 50%, transparent 100%);
	}
</style>

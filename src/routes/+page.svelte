<script>
	import { fade } from 'svelte/transition';
	import Card from '$lib/Card.svelte';

	import image1 from '$lib/assets/Question 1.png';
	import image2 from '$lib/assets/Question 2.png';
	import image3 from '$lib/assets/Question 3.png';
	import image4 from '$lib/assets/Question 4.png';
	import image5 from '$lib/assets/Question 5.png';
	import image6 from '$lib/assets/Question 6.png';
	import image7 from '$lib/assets/Question 7.png';
	import image9 from '$lib/assets/Question 9.png';
	import image10 from '$lib/assets/Question 10.png';

	const data = [
		{
			id: 1,
			preText: '',
			postText: '',
			answer: 'international',
			image: image1
		},
		{
			id: 2,
			preText: '',
			postText: '',
			answer: 'chainsaw',
			image: image2
		},
		{
			id: 3,
			preText: '',
			postText: '',
			answer: 'reception',
			image: image3
		},
		{
			id: 4,
			preText: '',
			postText: '',
			answer: 'solved',
			image: image4
		},
		{
			id: 5,
			preText: '',
			postText: '',
			answer: 'corrosive',
			image: image5
		},
		{
			id: 6,
			preText: '',
			postText: '',
			answer: 'fireplace',
			image: image6
		},
		{
			id: 7,
			preText: '',
			postText: '',
			answer: 'zgtozn',
			image: image7
		},
		{
			id: 8,
			preText: '',
			postText: '',
			answer: 'andromeda',
			text: `
01010111 01100101 01101100 01101100 00100000 01100100 01101111 01101110 01100101
00101110 00100000 01011001 01101111 01110101 01110010 00100000 01101110 01100101
01111000 01110100 00100000 01100011 01101100 01110101 01100101 00100000 01101001
01110011 00111010 00001010 00110100 00111001 00100000 00110110 01000100 00100000
00110111 00110000 00100000 00110111 00110010 00100000 00110110 00110101 00100000
00110111 00110011 00100000 00110111 00110011 00100000 00110110 00111001 00100000
00110111 00110110 00100000 00110110 00110101 00100000 00110010 00110000 00100000
00110111 00111001 00100000 00110110 01000110 00100000 00110111 00110101 00100000
00110010 00110000 00100000 00110111 00110011 00100000 00110111 00110000 00100000
00110110 01000110 00100000 00110111 00110100 00100000 00110111 00110100 00100000
00110110 00110101 00100000 00110110 00110100 00100000 00110010 00110000 00100000
00110110 00111001 00100000 00110111 00110100 00100000 00110010 00110000 00100000
00110111 00110111 00100000 00110110 00110001 00100000 00110111 00110011 00100000
00110010 00110000 00100000 00110110 00111000 00100000 00110110 00110101 00100000
00110111 00111000 00100000 00110110 00110001 00100000 00110110 00110100 00100000
00110110 00110101 00100000 00110110 00110011 00100000 00110110 00111001 00100000
00110110 01000100 00100000 00110110 00110001 00100000 00110110 01000011 00100000
00110010 00110000 00100000 00110010 01000100 00100000 00110010 00110000 00100000
00110111 00110100 00100000 00110110 00111000 00100000 00110110 00110101 00100000
00110010 00110000 00100000 00110110 01000101 00100000 00110110 00110101 00100000
00110111 00111000 00100000 00110111 00110100 00100000 00110010 00110000 00100000
00110110 00110011 00100000 00110110 01000110 00100000 00110110 00110100 00100000
00110110 00110101 00100000 00110010 00110000 00100000 00110111 00110111 00100000
00110110 00111001 00100000 00110110 01000011 00100000 00110110 01000011 00100000
00110010 00110000 00100000 00110110 00110111 00100000 00110110 00111001 00100000
00110111 00110110 00100000 00110110 00110101 00100000 00110010 00110000 00100000
00110111 00111001 00100000 00110110 01000110 00100000 00110111 00110101 00100000
00110010 00110000 00100000 00110111 00110100 00100000 00110110 00111000 00100000
00110110 00110101 00100000 00110010 00110000 00100000 00110111 00110011 00100000
00110110 01000110 00100000 00110110 01000011 00100000 00110111 00110101 00100000
00110111 00110100 00100000 00110110 00111001 00100000 00110110 01000110 00100000
00110110 01000101 00100000 00110011 01000001 00100000 00110000 01000001 00100000
00110010 01000101 00100000 00110010 01000100 00100000 00110010 00110000 00100000
00110010 01000100 00100000 00110010 01000101 00100000 00110010 00110000 00100000
00110010 01000100 00100000 00110010 01000101 00100000 00110010 01000101 00100000
00110010 00110000 00100000 00110010 01000101 00100000 00110010 01000100 00100000
00110010 01000101 00100000 00110010 00110000 00100000 00110010 01000100 00100000
00110010 01000100 00100000 00110010 01000100 00100000 00110010 00110000 00100000
00110010 01000100 00100000 00110010 01000100 00100000 00110010 00110000 00100000
00110010 01000101 00100000 00110010 00110000 00100000 00110010 01000100 00100000
00110010 01000101 00100000 00110010 01000101 00100000 00110010 00110000 00100000
00110010 01000101 00100000 00110010 01000100`
		},
		{
			id: 9,
			preText: '',
			postText: '',
			answer: 'bettyc7',
			image: image9
		},
		{
			id: 10,
			preText: '',
			postText: '',
			answer: '9876',
			image: image10
		}
	];

	let currentStage = $state(0);
	// $inspect(currentStage);

	let maxStage = $state(0);
	let maxAnswer = $state('');

	$effect(() => {
		maxStage = Math.max(maxStage, currentStage);
	});

	$effect(() => {
		maxAnswer = data[maxStage - 2]?.answer || '';
	});

	let currentProgress = $derived(Math.max((currentStage - 1) / data.length, 0));

	// Answer
	let currentAnswer = $state('');
	// $inspect(currentAnswer);

	let currentCode = $state('');
	// $inspect(currentCode);

	// Error
	let showError = $state(false);

	function checkAnswer(answer) {
		if (String(currentAnswer).toLowerCase().trim() !== String(answer).toLowerCase().trim()) {
			showError = true;

			// Hide error after 3 seconds
			setTimeout(() => {
				showError = false;
			}, 3000);
		} else {
			goForward(true);
			currentCode = answer;
			currentAnswer = '';
		}
	}

	function goForward(progress) {
		switch (true) {
			case currentStage >= maxStage && progress:
				currentStage = Math.max(Math.min(currentStage + 1, data.length + 1), 0);
				break;
			case currentStage < maxStage:
				currentStage = Math.max(Math.min(currentStage + 1, data.length + 1), 0);
				break;
			default:
				break;
		}
	}

	function goBack() {
		currentStage = Math.max(Math.min(currentStage - 1, data.length), 0);
	}

	function goToStage(code) {
		// check if any of the answers match the code
		const stage = data.find(
			(datum) => datum.answer.toLowerCase().trim() === code.toLowerCase().trim()
		);
		if (stage) {
			currentStage = stage.id + 1;
			// currentCode = '';
		}
	}

	function handleCopy(text) {
		console.log('Copying', text);
		navigator.clipboard.writeText(text);
	}
</script>

<div>{currentProgress * 100 + '%'}</div>
<div class="progress-bar" style={`--progress-percentage: ${currentProgress * 100}%`}></div>
<div class="controls">
	<button onclick={goBack}><span class="material-symbols-outlined"> arrow_back </span></button>
	<form
		onsubmit={(e) => {
			e.preventDefault();
			goToStage(currentCode);
		}}
	>
		<input type="text" bind:value={currentCode} placeholder="Previous Answer" />
	</form>
	<button onclick={() => goForward()} disabled={currentStage >= maxStage}
		><span class="material-symbols-outlined"> arrow_forward </span></button
	>
</div>
{#if currentStage === 0}
	<Card>
		<h1>Are you ready for your quiz?</h1>
		<button
			onclick={() => {
				currentStage++;
			}}>Let's go!</button
		>
	</Card>
{:else if currentStage >= 0 && currentStage <= data.length}
	{#each data as datum, i}
		{#if currentStage === datum.id}
			<Card>
				{#if datum.image}
					<img src={datum.image} alt="Question" />
				{:else if datum.text}
					<div class="binary-container">
						<pre class="binary-content">{datum.text}</pre>
						<button class="copy-button" onclick={() => handleCopy(datum.text)}> Copy </button>
					</div>
				{/if}

				<form
					class="input"
					onsubmit={(e) => {
						e.preventDefault();
						checkAnswer(datum.answer);
					}}
				>
					<input type="text" bind:value={currentAnswer} placeholder="Answer here" autofocus />

					<div class="feedback-container">
						{#if showError}
							<div in:fade={{ duration: 250 }} out:fade={{ duration: 1000 }} class="feedback">
								Incorrect Answer
							</div>
						{/if}
					</div>
				</form>

				<button disabled={!currentAnswer} onclick={() => checkAnswer(datum.answer)}
					>Check Answer</button
				>
			</Card>
		{/if}
	{/each}
{:else if currentStage > data.length}
	<Card>
		<h1>Well done! You've completed the quiz!</h1>
		<h2>The code to the lock is <b>{data[data.length - 1]?.answer}</b></h2>
		<button
			onclick={() => {
				currentStage = 0;
			}}>Restart</button
		>
	</Card>
{:else}
	<p>Something went wrong</p>
{/if}

<style>
	.controls {
		display: flex;
		min-width: 40rem;
		max-width: 90vw;
		justify-content: space-between;
	}

	.progress-bar {
		--progress-background: #eee;
		--progress-fill: #2196f3;
		--progress-width: 300px;
		--progress-height: 20px;
		--progress-percentage: 50%; /* Change this percentage to adjust progress */

		width: var(--progress-width);
		height: var(--progress-height);
		background: linear-gradient(
			to right,
			var(--progress-fill) var(--progress-percentage),
			var(--progress-background) var(--progress-percentage)
		);
		border-radius: calc(var(--progress-height) / 2);
	}

	img {
		width: 100%;
		height: auto;
		max-height: 80vh;
		border-radius: 1rem;
		border: solid black 2px;
	}

	.input {
		display: flex;
		flex-direction: column;
		/* width: 100%; */
		/* background-color: pink; */
	}

	.feedback-container {
		height: 1rem;
		margin: 0.25rem;
		/* background-color: pink; */
	}

	.feedback {
		color: #0d5a99;
		font-weight: bold;
	}

	.binary-container {
		display: flex;
		flex-direction: column;
		position: relative;
		border-radius: 8px;
		border: 1px solid #e2e8f0;
		background-color: white;
		color: black;
		padding: 16px;
		box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
	}

	.binary-content {
		margin: 0;
		padding: 0;
		font-family: ui-monospace, monospace;
		white-space: pre-wrap;
		overflow-x: auto;
	}

	.copy-button {
		/* position: absolute; */
		/* top: 8px;
		right: 8px; */
		padding: 4px 8px;
		margin: 16px;
		border-radius: 4px;
		font-size: 16px;
		font-weight: 500;
		letter-spacing: 0.1em;
		text-transform: uppercase;
		color: #1e293b;
		background-color: #dbeafe;
		border: none;
		cursor: pointer;
		transition: all 0.2s ease;
	}

	.copy-button:hover {
		background-color: #bfdbfe;
		color: #1e40af;
	}

	b {
		color: #0d5a99;
		font-weight: bold;
	}
</style>

<script>
	// import svelteLogo from './assets/svelte.svg'
	// import Counter from './lib/Counter.svelte'
	const firstName = "Adeniyi";
	const lastName = "Aderinto";
	const statement = "<em>EsQ<em/>";
	const age = 49;
	const names = ["Bruce", "akin", "diana"];
</script>

<main>
	<h1>Hello {firstName} omo {lastName} {@html statement}</h1>
	{#if age > 50}
		<h3>You are a middle aged man</h3>
	{:else if age < 50}
		<h3>Young Omo professor agba</h3>
	{/if}
</main>
{#each names as item}
	<h2>{item}</h2>
{/each}

<style>
	.logo {
		height: 6em;
		padding: 1.5em;
		will-change: filter;
	}
	.logo:hover {
		filter: drop-shadow(0 0 2em #646cffaa);
	}
	.logo.svelte:hover {
		filter: drop-shadow(0 0 2em #ff3e00aa);
	}
	.read-the-docs {
		color: #888;
	}
</style>

<script lang="ts">
	export let name: string;
	export let rawDate: string;
	const time = new Date(rawDate);
</script>

<svelte:head>
	<title>{name}</title>
</svelte:head>

<main>
	<h1>{name}</h1>
	<p>Matt Gleich -> {`${time.getMonth() + 1}/${time.getDate() + 1}/${time.getFullYear()}`}</p>
	<slot class="slot" />
</main>

<style>
	main {
		margin-bottom: 50px;
		margin-top: 30vh;
		margin-left: 20px;
		margin-right: 20px;
		width: 1000px;
		max-width: 1000px;
	}
</style>

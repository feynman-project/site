<script lang="ts">
	export let name: String;
	export let date: Date;
</script>

<main>
	<h1>{name}</h1>
	<p>Matt Gleich -> {`${date.getMonth()}/${date.getDate()}/${date.getFullYear()}`}</p>
	<slot class="slot" />
</main>

<style>
	main {
		margin-bottom: 50px;
		margin-top: 30vh;
		margin-left: 20px;
		margin-right: 20px;
		max-width: 1000px;
	}
</style>

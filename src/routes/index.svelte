<script>
	import Logo from '../components/Logo.svelte';
</script>

<main>
	<div class="left">
		<Logo />
	</div>
	<div class="right">
		<h1>Feynman Project</h1>
		<p>
			<a href="https://en.wikipedia.org/wiki/Richard_Feynman">Richard Feynman</a> is one of the most
			influential and important physicists of the last century. Outside of his innovative research in
			the world of quantum mechanics, he was also an amazing teacher, giving his students a deep and
			natural understanding of physics. This project aims to create physics teaching material to give
			students a deeper understanding of physics at the high school level.
		</p>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-wrap: wrap;
		margin: 0 20px;
	}

	.left {
		padding-right: 30px;
	}

	h1 {
		margin-top: 15px;
	}

	p {
		max-width: 600px;
	}
</style>

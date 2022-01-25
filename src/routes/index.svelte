<script>
	import Logo from '../components/Logo.svelte';
</script>

<svelte:head>
	<title>Feynman Project</title>
</svelte:head>

<main>
	<div class="left">
		<Logo />
		<br />
		<p>&copy; {new Date().getFullYear()} <a href="https://mattglei.ch">Matt Gleich</a></p>
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
		<h2>Circuits</h2>
		<p>
			Custom made PCBs to help students understand voltage, current, and resistance all a number of
			difference circuits. Check out the <a href="https://github.com/feynman-project/circuits"
				>github repository</a
			> to learn more.
		</p>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-wrap: wrap;
	}

	.left {
		padding-right: 30px;
		display: flex;
		flex-direction: column;
		align-items: flex-end;
	}

	h1 {
		margin-top: 15px;
	}

	p {
		max-width: 600px;
	}
</style>

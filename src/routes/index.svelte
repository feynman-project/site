<script>
	import Logo from '../components/Logo.svelte';
</script>

<svelte:head>
	<title>Feynman Project</title>
	<meta name="description" content="Transformative tools for teaching physics" />
	<meta property="og:title" content="Feynman Project" />
	<meta property="og:description" content="Transformative tools for teaching physics" />
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
			Custom made PCBs to help students understand voltage, current, and resistance all in a number
			of different circuits types (e.g. series, parallel, RC). Check out the <a
				href="https://github.com/feynman-project/circuits">github repository</a
			> to follow the development. Here are the development logs:
		</p>
		<ol>
			<li><a href="/logs/circuits/init">Initial Plan</a> -> January 25<sup>th</sup>, 2022</li>
			<li><a href="/logs/circuits/01">Update #1</a> -> February 18<sup>th</sup>, 2022</li>
		</ol>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-wrap: wrap;
		margin: 0 20px;
		margin-top: 30vh;
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

	ol {
		list-style-type: upper-roman;
	}

	@media screen and (max-width: 793px) {
		main {
			margin-top: 20vh;
		}

		.left {
			padding-left: 10px;
			flex-direction: row;
			gap: 20px;
		}
	}
</style>

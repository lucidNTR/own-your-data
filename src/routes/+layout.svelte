<script>
	import '../app.css';
	let y = 0;
</script>

<svelte:window bind:scrollY={y} />

<header class:scrolled={y > 20}>
	<h1><a href="/">Own-Your-Data.org</a></h1>
	<nav>
		<a href="/services">Services</a>
	</nav>
</header>

<main>
	<slot />
</main>

<footer>
	<p>
		&copy; 2025 Own-Your-Data.org &mdash; Take Back Control
	</p>
</footer>

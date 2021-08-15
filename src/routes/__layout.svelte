<script>
	import '../global.css';
	import Nav from '$lib/Nav.svelte';
</script>

<header>
	<h1>Josh Suson</h1>
	<Nav />
</header>
<main>
	<slot />
</main>
<footer>© 2021</footer>

<style>
	:global(body) {
		background-color: var(--black);
	}
</style>

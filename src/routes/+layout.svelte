<script>
import { base } from '$app/paths';
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>


<nav>
	<a href="{base}/">Accueil</a> |
	<a href="{base}/about">À propos</a> |
	<a href="{base}/contact">Contact</a>
</nav>

<main>
	{@render children()}
</main>

<style>
	nav { padding: 1rem; background: #f4f4f4; }
	main { padding: 2rem; font-family: sans-serif; }
</style>
<script>
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<nav>
	<a href="/">Home</a>
	<a href="/about">About</a>
</nav>
{@render children?.()}

<style>
	nav {
		background: gray;
		padding: 10px;
	}

	nav a {
		color: white;
	}
</style>

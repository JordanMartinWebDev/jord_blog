<script>
	import '$lib/styles/style.scss';
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import '@fontsource-variable/inter';
	import bracketOpen from '$lib/assets/Logo Open.svg';
	import bracketClose from '$lib/assets/Logo Close.svg';
</script>

<Header />

<main>
	<img alt="bracket open" src={bracketOpen} class="curly" />
	<slot />
	<img alt="bracket close" src={bracketClose} class="curly" />
</main>

<Footer />

<style>
	main {
		margin: 5rem auto;
		max-width: 90%;
		display: block;
	}
</style>

<script>
	import Footer from '$lib/Footer.svelte';
	import Header from '$lib/Header.svelte';
	import '../app.css';

	let { children } = $props();
</script>

<div>
	<div class="container mx-auto px-2">
		<Header />
		<main>
			{@render children()}
		</main>
	</div>
	<Footer />
</div>

<script>
	import Footer from '$lib/Footer.svelte';
	import Header from '$lib/Header.svelte';
	import '../styles.css';
</script>

<div>
	<div class="container mx-auto px-2">
		<Header />
		<main>
			<slot />
		</main>
	</div>
	<Footer />
</div>

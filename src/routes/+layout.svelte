<script>
	import Header from '$lib/Header.svelte';
	import '../styles.css';
</script>

<div class="container mx-auto px-2">
	<Header />
	<main>
		<slot />
	</main>
</div>

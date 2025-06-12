<script>
	import ProjectCard from '$lib/ProjectCard.svelte';

	import ren from '$lib/images/ren.webp';
</script>

<h2 id="clients" class="text-primary mb-12 w-fit border-b border-white/80 text-4xl">Clients</h2>
<div class="mb-32 flex flex-col space-y-32">
	<ProjectCard
		subtitle="Contractors"
		title="Renovation and Revamp"
		image={ren}
		primaryBtnLink="https://renovationandrevamp.com"
		primaryBtnText="View website"
		description="A modern, responsive marketing website for a local building contractor, designed to highlight services, showcase client reviews, and establish credibility. Built with SvelteKit and fully server-rendered for SEO and performance, the site includes an image carousel, Google Reviews integration. Deployed on a Linux server with Nginx and secured with SSL via Certbot."
	/>
</div>

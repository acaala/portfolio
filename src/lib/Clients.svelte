<script>
	import ProjectCard from '$lib/ProjectCard.svelte';

	import ren from '$lib/images/ren.png';
</script>

<h2 id="clients" class="text-primary mb-12 w-fit border-b border-white/80 text-4xl">Clients</h2>
<div class="mb-32 flex flex-col space-y-32">
	<ProjectCard
		subtitle="Contractors"
		title="Renovation and Revamp"
		image={ren}
		primaryBtnLink="https://renovationandrevamp.com"
		primaryBtnText="View website"
		description="Built using Svelte"
	/>
</div>

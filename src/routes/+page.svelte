<script>
	import ProjectCard from '$lib/ProjectCard.svelte';
	import Github from '$lib/icons/Github.svelte';
	import Linkedin from '$lib/icons/Linkedin.svelte';
</script>

<div>
	<div class="mb-12">
		<div class="text-center md:text-left my-32 px-4 md:px-0">
			<h1 class="uppercase text-5xl text-primary leading-normal">
				Creating Unique <br />Experiences
			</h1>
		</div>

		<div class="flex items-center w-full justify-between px-4 md:px-0">
			<div class="divider h-0.5 bg-gray-200 w-3/4"></div>
			<a href="https://github.com/acaala"><Github /></a>
			<a href="https://www.linkedin.com/in/lawatts1/"><Linkedin /></a>
		</div>
	</div>

	<div class=""></div>
	<ProjectCard />
</div>

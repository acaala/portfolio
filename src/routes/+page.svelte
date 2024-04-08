<script>
	import { onMount } from 'svelte';
	import ProjectCard from '$lib/ProjectCard.svelte';
	import Github from '$lib/icons/Github.svelte';
	import Linkedin from '$lib/icons/Linkedin.svelte';
	import HeroShapes from '$lib/HeroShapes.svelte';
	import { gsap } from 'gsap';

	onMount(() => {
		const t1 = gsap.timeline();

		t1.from('#hero-content', { duration: 3, x: -300, opacity: 0 });
	});
</script>

<div>
	<div class="mb-12">
		<div class="flex justify-between my-32 items-center">
			<div id="hero-content" class="text-center md:text-left px-4 md:px-0">
				<h1 class="uppercase text-5xl text-primary leading-normal">
					Creating Unique <br />Experiences
				</h1>
			</div>
			<HeroShapes />
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

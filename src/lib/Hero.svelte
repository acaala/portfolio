<script>
	import HeroShapes from './HeroShapes.svelte';
	import Scroll from './Scroll.svelte';
	import Github from './icons/Github.svelte';
	import Linkedin from './icons/Linkedin.svelte';
	import { onMount } from 'svelte';
	import { gsap } from 'gsap';

	onMount(() => {
		const t1 = gsap.timeline();

		t1.from('#hero-content', { duration: 3, x: -300, opacity: 0 });
	});
</script>

<div class="my-32 flex items-center justify-center md:justify-between">
	<div id="hero-content" class="px-4 text-center md:px-0 md:text-left">
		<h1 class="text-primary text-5xl leading-normal uppercase">
			Creating Unique <br />Experiences
		</h1>
		<div class="mt-5 flex items-center justify-center md:justify-start">
			<Scroll />
			<p class="text-primary px-5 text-sm tracking-widest uppercase">Scroll for more!</p>
		</div>
	</div>
	<div class="hidden md:block">
		<HeroShapes />
	</div>
</div>
<div class="flex w-full items-center justify-between px-4 md:px-0">
	<div class="divider h-0.5 w-3/4 bg-gray-200"></div>
	<a href="https://github.com/acaala"><Github /></a>
	<a href="https://www.linkedin.com/in/lawatts1/"><Linkedin /></a>
</div>

<script>
	import { onMount } from 'svelte';
	import { gsap } from 'gsap';

	import ProjectCard from '$lib/ProjectCard.svelte';
	import Github from '$lib/icons/Github.svelte';
	import Linkedin from '$lib/icons/Linkedin.svelte';
	import HeroShapes from '$lib/HeroShapes.svelte';
	import Scroll from '$lib/Scroll.svelte';

	import coinseekerImage from '$lib/images/coinseeker.png';
	import rustoneImage from '$lib/images/rustone.png';

	onMount(() => {
		const t1 = gsap.timeline();

		t1.from('#hero-content', { duration: 3, x: -300, opacity: 0 });
	});
</script>

<div>
	<div class="mb-32">
		<div class="flex md:justify-between my-32 items-center justify-center">
			<div id="hero-content" class="text-center md:text-left px-4 md:px-0">
				<h1 class="uppercase text-5xl text-primary leading-normal">
					Creating Unique <br />Experiences
				</h1>
				<div class="flex mt-5 items-center justify-center md:justify-start">
					<Scroll />
					<p class="tracking-widest text-sm uppercase px-5 text-primary">Scroll for more!</p>
				</div>
			</div>
			<div class="hidden md:block">
				<HeroShapes />
			</div>
		</div>

		<div class="flex items-center w-full justify-between px-4 md:px-0">
			<div class="divider h-0.5 bg-gray-200 w-3/4"></div>
			<a href="https://github.com/acaala"><Github /></a>
			<a href="https://www.linkedin.com/in/lawatts1/"><Linkedin /></a>
		</div>
	</div>

	<div id="projects" class="flex flex-col space-y-32 mb-32">
		<ProjectCard
			subtitle="Featured Project"
			title="Rustone"
			image={rustoneImage}
			primaryBtnLink="https://github.com/acaala/rustone"
			primaryBtnText="Github Repo"
			description="An AI-powered guitar amp simulator in Rust using Tauri, inspired by Guitar Rig and Amplitube, dynamically generates setups based on user inputs."
		/>

		<ProjectCard
			subtitle="Past project"
			title="Coinseeker"
			image={coinseekerImage}
			primaryBtnLink="https://coinseeker.liamw.dev"
			secondaryBtnLink="https://github.com/acaala/coinseeker"
			description="A Nuxt.JS app using Composition-api and TailwindCSS. Fetches live price data for
		cryptocurrencies, user can search for a single coin and can covert to a different currency."
		/>
	</div>
</div>

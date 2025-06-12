<script>
	import ProjectCard from '$lib/ProjectCard.svelte';

	import deepRiff from '$lib/images/deep-riff.webp';
	import quickReplaceImage from '$lib/images/quick-replace.png';
	import rcv from '$lib/images/rcv.mp4';
</script>

<h2 id="projects" class="text-primary mb-12 w-fit border-b border-white/80 text-4xl">Projects</h2>
<div class="mb-32 flex flex-col space-y-32">
	<ProjectCard
		subtitle="Featured Project"
		title="Deep Riff"
		image={deepRiff}
		description="An AI-powered guitar amp simulator in Rust using Tauri, inspired by Guitar Rig and Amplitube, dynamically generates setups based on user inputs."
	/>

	<ProjectCard
		subtitle="CLI Project"
		title="RCV"
		video={rcv}
		primaryBtnLink="https://github.com/acaala/rcv-cli"
		primaryBtnText="Github repo"
		description="Multi Threaded Image Converter - Efficiently convert images to WebP format with customisable compression settings. "
	/>

	<ProjectCard
		subtitle="Past project"
		title="Quick Replace"
		image={quickReplaceImage}
		primaryBtnLink="https://quick-replace.liamw.dev"
		secondaryBtnLink="https://github.com/acaala/quick_replace"
		description="A fast find and replace tool leveraging websockets for real time replacement updates. Both the CLI tool and the Webserver are written in Rust"
	/>
</div>

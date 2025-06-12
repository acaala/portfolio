<script>
	import { onMount } from 'svelte';
	import gsap from 'gsap';

	onMount(() => {
		const t3 = gsap.timeline();
		t3.to('#scroll-circle', {
			duration: 3,
			yPercent: 150,
			yoyo: true,
			repeat: -1,
			ease: 'circ'
		});
	});
</script>

<div>
	<svg xmlns="http://www.w3.org/2000/svg" width="35" height="90" viewBox="0 0 51 91">
		<g id="scroll-svg" transform="translate(-233 -685)">
			<g
				id="Rectangle_1"
				data-name="Rectangle 1"
				transform="translate(233 685)"
				fill="none"
				stroke="#fff"
				stroke-width="5"
			>
				<rect width="51" height="91" rx="25.5" stroke="none" />
				<rect x="2.5" y="2.5" width="46" height="86" rx="23" fill="none" />
			</g>
			<g
				id="scroll-circle"
				data-name="Ellipse 1"
				transform="translate(242 695)"
				fill="#fff"
				stroke="#fff"
				stroke-width="1"
			>
				<ellipse cx="16.5" cy="15" rx="16.5" ry="15" stroke="none" />
				<ellipse cx="16.5" cy="15" rx="16" ry="14.5" fill="none" />
			</g>
		</g>
	</svg>
</div>

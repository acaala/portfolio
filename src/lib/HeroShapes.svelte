<script>
	import gsap from 'gsap';
	import { onMount } from 'svelte';

	onMount(() => {
		const t2 = gsap.timeline();

		t2.from('.col-1', {
			duration: 2,
			opacity: 0,
			y: -100,
			stagger: 0.3,
			ease: 'bounce'
		}).from(
			'.col-2',
			{
				duration: 2,
				opacity: 0,
				y: -100,
				stagger: 0.4,
				ease: 'bounce'
			},
			'=-3.2'
		);
	});
</script>

<div>
	<svg xmlns="http://www.w3.org/2000/svg" width="280" height="560" viewBox="0 0 280 560">
		<g id="hero-img" transform="translate(-1127 -252)">
			<rect
				class="col-2 row-1"
				id="purple-sq-1"
				data-name="Rectangle 2"
				width="140"
				height="140"
				rx="22"
				transform="translate(1267 252)"
				fill="#a16ae8"
			/>
			<circle
				class="col-1 row-1"
				id="white-circle-2"
				data-name="Ellipse 3"
				cx="70"
				cy="70"
				r="70"
				transform="translate(1127 252)"
				fill="#fff"
			/>
			<rect
				class="col-2 row-3"
				id="purple-sq-2"
				data-name="Rectangle 7"
				width="140"
				height="140"
				rx="22"
				transform="translate(1267 532)"
				fill="#a16ae8"
			/>
			<rect
				class="col-1 row-2"
				id="green-sq-1"
				data-name="Rectangle 4"
				width="140"
				height="140"
				rx="22"
				transform="translate(1127 392)"
				fill="#4cfcd3"
			/>
			<rect
				class="col-1 row-4"
				id="green-sq-2"
				data-name="Rectangle 8"
				width="140"
				height="140"
				rx="22"
				transform="translate(1127 672)"
				fill="#4cfcd3"
			/>
			<circle
				class="col-1 row-3"
				id="white-circle-1"
				data-name="Ellipse 2"
				cx="70"
				cy="70"
				r="70"
				transform="translate(1127 532)"
				fill="#fff"
			/>
			<circle
				class="col-2 row-2"
				id="pink-circle-1"
				data-name="Ellipse 4"
				cx="70"
				cy="70"
				r="70"
				transform="translate(1267 392)"
				fill="#fd49a0"
			/>
			<circle
				class="col-2 row-4"
				id="pink-circle-2"
				data-name="Ellipse 5"
				cx="70"
				cy="70"
				r="70"
				transform="translate(1267 672)"
				fill="#fd49a0"
			/>
		</g>
	</svg>
</div>

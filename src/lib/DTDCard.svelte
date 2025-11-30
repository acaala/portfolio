<script>
	import dtd from '$lib/images/dtd/DTD_Live.webp';
	import coinrivet from '$lib/images/dtd/coinrivet.webp';
	import luxon from '$lib/images/dtd/luxon.webp';

	import dtdLogo from '$lib/images/dtd/dtd-logo-white.webp';
	import luxonLogo from '$lib/images/dtd/luxon-logo.webp';
	import coinrivetLogo from '$lib/images/dtd/coinrivet-logo.webp';
	import appStore from '$lib/images/dtd/app-store.svg';
	import playStore from '$lib/images/dtd/googleplay.svg';
	import shotclockApp from '$lib/images/dtd/shotclock_appstore.webp';
	import shotclockPlay from '$lib/images/dtd/shotclock_googleplay.webp';

	let hovered = null;

	const onHover = (id) => (hovered = id);
	const onLeave = () => (hovered = null);
</script>

<div class="container items-center justify-center rounded-xl bg-white px-5 py-10 lg:flex">
	<div class="mx-auto mb-2 p-2 text-center md:mb-0 lg:mx-4 lg:w-1/3 lg:text-left">
		<h2 class="text-secondary text-xs tracking-widest uppercase lg:text-sm">
			Gaming, Finance & Internal Platforms
		</h2>

		<h3 class="text-2xl font-medium uppercase xl:text-3xl">DTD Live</h3>

		<p class="my-4 leading-relaxed text-gray-900">
			Supported multiple brands under a single client by delivering high-quality websites and
			essential internal tools. Improved workflows, modernized outdated systems, and implemented
			reliable, scalable solutions across different business units.
		</p>

		<div class="my-4 flex justify-center space-x-2 lg:justify-start lg:space-x-4">
			<a
				target="_blank"
				onmouseenter={() => onHover('dtd')}
				onmouseleave={onLeave}
				href="https://dusktilldawnpoker.com"
				class="h-12 w-12 rounded-lg bg-zinc-900 p-2 shadow hover:bg-zinc-950"
			>
				<img src={dtdLogo} alt="DTD" class=" h-full w-full object-contain" />
			</a>
			<a
				target="_blank"
				onmouseenter={() => onHover('luxon')}
				onmouseleave={onLeave}
				href="https://luxon.com"
				class="h-12 w-12 rounded-lg bg-zinc-900 p-2 shadow hover:bg-zinc-950"
			>
				<img src={luxonLogo} alt="luxon" class="h-full w-full object-contain" />
			</a>
			<a
				target="_blank"
				onmouseenter={() => onHover('coinrivet')}
				onmouseleave={onLeave}
				href="https://coinrivet.com"
				class="h-12 w-12 rounded-lg bg-zinc-900 p-2 shadow hover:bg-zinc-950"
			>
				<img src={coinrivetLogo} alt="coinrivet" class="h-full w-full object-contain" />
			</a>
		</div>
		<div class="flex items-center justify-center gap-2 lg:justify-start">
			<a
				target="_blank"
				onmouseenter={() => onHover('appstore')}
				onmouseleave={onLeave}
				href="https://apps.apple.com/uy/app/dtd-shotclock/id6744166846"
				class="w-32 rounded-lg"
			>
				<img src={appStore} alt="coinrivet" class="object-contain" />
			</a>
			<a
				target="_blank"
				onmouseenter={() => onHover('playstore')}
				onmouseleave={onLeave}
				href="https://play.google.com/store/apps/details?id=com.dtd.shot_clock&hl=en"
				class="w-32 rounded-lg"
			>
				<img src={playStore} alt="coinrivet" class="object-contain" />
			</a>
		</div>
	</div>
	<div class="bg-primary mx-auto w-full overflow-hidden rounded-3xl shadow-md md:w-2/3 lg:ml-5">
		<div
			class="relative h-[300px] w-full rounded-2xl [perspective:1400px] lg:h-[360px] xl:h-[500px]"
		>
			<img src={dtd} alt="DTD" class:active={hovered == 'dtd'} class="card -left-0 z-30" />
			<img
				class:active={hovered == 'luxon'}
				id="luxon"
				src={luxon}
				alt="Luxon"
				class="card left-1/12 z-20 hover:z-50"
			/>
			<img
				class:active={hovered == 'coinrivet'}
				src={coinrivet}
				alt="Coinrivet"
				class="card left-2/12"
			/>
			<img
				class:active={hovered == 'appstore'}
				src={shotclockApp}
				alt="Shotclock AppStore"
				class="card left-3/12 -z-10 hover:z-100"
			/>
			<img
				class:active={hovered == 'playstore'}
				src={shotclockPlay}
				alt="Shotclock Google Play"
				class="card left-4/12 -z-20 hover:z-100"
			/>
		</div>
	</div>
</div>

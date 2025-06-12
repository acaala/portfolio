<script>
	export let subtitle;
	export let title;
	export let description;
	export let image = '';
	export let video = '';
	export let primaryBtnLink = '';
	export let primaryBtnText = 'Take Me There';
	export let secondaryBtnLink = '';
	export let secondaryBtnText = 'Github Repo';
</script>

<div class="container items-center justify-center rounded-xl bg-white px-5 py-10 lg:flex">
	<div class="mx-auto mb-2 p-2 text-center md:mb-0 lg:mx-4 lg:w-1/3 lg:text-left">
		<h2 class="text-secondary text-xs tracking-widest uppercase lg:text-sm">{subtitle}</h2>

		<h3 class="text-2xl font-medium uppercase xl:text-3xl">{title}</h3>

		<p class="my-4 leading-relaxed text-gray-900">
			{description}
		</p>

		<div
			class="my-4 flex justify-center space-x-10 text-center lg:max-w-48 lg:flex-col lg:space-y-4 lg:space-x-0"
		>
			{#if primaryBtnLink}
				<a
					class="border-secondary bg-secondary hover:text-secondary rounded-full border px-5 py-1 text-white hover:bg-white"
					href={primaryBtnLink}>{primaryBtnText}</a
				>
			{/if}
			{#if secondaryBtnLink}
				<a
					class="border-tertiary text-tertiary hover:bg-tertiary rounded-full border bg-white px-5 py-1 hover:text-white"
					href={secondaryBtnLink}>{secondaryBtnText}</a
				>
			{/if}
		</div>
	</div>
	<div
		class="bg-primary mx-auto w-full overflow-hidden rounded-3xl pt-2 pr-2 shadow-md md:w-2/3 lg:ml-5"
	>
		{#if video}
			<video
				autoplay
				muted
				loop
				playsinline
				width="100%"
				height="auto"
				class="max-h-[400px] w-full rounded-2xl object-cover object-top lg:max-h-[500px]"
			>
				<source src={video} type="video/mp4" />
			</video>
		{:else}
			<img
				class="h-full max-h-[400px] w-full rounded-2xl object-cover object-top lg:max-h-[500px]"
				src={image}
				alt={title}
			/>
		{/if}
	</div>
</div>

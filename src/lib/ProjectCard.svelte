<script lang="ts">
	export let subtitle: string;
	export let title: string;
	export let description: string;
	export let image: string;
	export let primaryBtnLink = '';
	export let primaryBtnText = 'Take Me There';
	export let secondaryBtnLink = '';
	export let secondaryBtnText = 'Github Repo';
</script>

<div class="bg-white container rounded-xl items-center px-5 py-10 lg:flex justify-center">
	<div class="mx-auto text-center p-2 mb-2 md:mb-0 lg:text-left lg:mx-4 lg:w-1/3">
		<h2 class="uppercase tracking-widest text-xs lg:text-sm text-secondary">{subtitle}</h2>

		<h3 class="uppercase text-2xl xl:text-3xl font-medium">{title}</h3>

		<p class="leading-relaxed text-gray-900 my-4">
			{description}
		</p>

		<div
			class="flex space-x-10 text-center justify-center my-4 lg:flex-col lg:space-y-4 lg:space-x-0 lg:max-w-48"
		>
			{#if primaryBtnLink}
				<a
					class="border border-secondary text-white bg-secondary px-5 py-1 rounded-full hover:bg-white hover:text-secondary"
					href={primaryBtnLink}>{primaryBtnText}</a
				>
			{/if}
			{#if secondaryBtnLink}
				<a
					class="border border-tertiary bg-white text-tertiary px-5 py-1 rounded-full hover:bg-tertiary hover:text-white"
					href={secondaryBtnLink}>{secondaryBtnText}</a
				>
			{/if}
		</div>
	</div>
	<div class="bg-primary rounded-3xl pt-2 w-full pr-2 md:w-2/3 lg:ml-5 shadow-md mx-auto">
		<img
			class="rounded-2xl max-h-[400px] h-full object-cover w-full object-top lg:max-h-[500px]"
			src={image}
			alt={title}
		/>
	</div>
</div>

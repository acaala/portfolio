<script>
	import image from '$lib/images/coinseeker.png';
</script>

<div class="bg-white container rounded-xl items-center px-5 py-10 lg:flex">
	<div class="mx-auto text-center p-2 mb-2 md:mb-0 lg:text-left lg:mx-4 lg:w-1/3">
		<h2 class="uppercase tracking-widest text-xs lg:text-sm text-secondary">Past Project</h2>

		<h3 class="uppercase text-2xl xl:text-3xl font-medium">Coinseeker</h3>

		<p class="leading-relaxed text-gray-900 my-4">
			A Nuxt.JS app using Composition-api and TailwindCSS. Fetches live price data for
			cryptocurrencies, user can search for a single coin and can covert to a different currency.
		</p>

		<div
			class="flex space-x-10 text-center justify-center my-4 lg:flex-col lg:space-y-4 lg:space-x-0 lg:max-w-48"
		>
			<a
				class="border border-secondary text-white bg-secondary px-5 py-1 rounded-full hover:bg-white hover:text-secondary"
				href="https://coinseeker.liamw.dev">Take Me There</a
			>
			<a
				class="border border-tertiary bg-white text-tertiary px-5 py-1 rounded-full hover:bg-tertiary hover:text-white"
				href="https://github.com/acaala/coinseeker">Github Repo</a
			>
		</div>
	</div>
	<div class="bg-primary rounded-3xl pt-2 w-full pr-2 md:w-2/3 lg:ml-5 shadow-md">
		<img
			class="rounded-2xl max-h-[400px] object-cover w-full object-top"
			src={image}
			alt="coinseeker"
		/>
	</div>
</div>

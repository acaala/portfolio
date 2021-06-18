<template>
  <div
    id="featured-project"
    class="container bg-white rounded-xl lg:flex items-center px-5 py-12 mt-32 shadow-2xl"
  >
    <!-- Text content -->
    <div
      id="featured-text"
      class="lg:w-1/3 mx-auto text-center lg:text-left lg:mx-4 px-2 mb-2 md:mb-0 py-2"
    >
      <h3 class="uppercase tracking-widest text-xs lg:text-sm font-medium">
        featured project
      </h3>
      
      <h2 class="uppercase text-2xl xl:text-3xl font-medium">
        Coinseeker.netlify.app
      </h2>
      
      <p class="leading-relaxed text-gray-900 my-4">A Nuxt.JS app using Composition-api and TailwindCSS. Fetches live price data for cryptocurrencies, user can search for a single coin and can covert to a different currency.</p>
      <a href="https://coinseeker.netlify.app" class="btn-primary">Take Me There</a>

    </div>
    <!-- Picture -->
    <div id="featured-image" class="md:w-2/3 lg:ml-5 shadow-md">
      <FeaturedImage />
    </div>
  </div>
</template>


<style lang="postcss" scoped>
h3 {
  color: #fd49a0;
}

#featured-image {
  background: #4cfcd3;

  @apply rounded-3xl pt-2 w-full pr-2;
}
</style>
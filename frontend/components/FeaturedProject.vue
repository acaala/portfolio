<template>
  <div
    id="featured-project"
    class="container bg-white rounded-xl lg:flex items-center px-5 py-12 my-12 shadow-2xl"
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
      <p class="leading-relaxed text-gray-900 my-4">A Nuxt.JS app</p>

      <!-- <button class="btn-secondary lg:mt-5 mx-auto mb-4">Take Me There</button> -->
    </div>
    <!-- Picture -->
    <div id="featured-image" class="md:w-2/3 lg:ml-5 shadow-md">
      <FeaturedImage />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, onMounted } from '@nuxtjs/composition-api'
export default defineComponent({
  setup() {
    onMounted(() => {
      const t5 = gsap.timeline()

      t5.from('#featured-text', {
        scrollTrigger: '#featured-project',
        start: 'bottom bottom',
        x: -200,
        duration: 3,
        opacity: 0,
      })
      t5.from(
        '#featured-image',
        {
          scrollTrigger: '#featured-project',
          x: 300,
          duration: 3,
          opacity: 0,
        },
        '-=3'
      )
    })
  },
})
</script>

<style lang="postcss" scoped>
h3 {
  color: #fd49a0;
}

#featured-image {
  background: #4cfcd3;

  @apply rounded-3xl pt-2 w-full pr-2;
}
</style>
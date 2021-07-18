<template>
  <div>
    <div class="container mx-auto px-2">
      <div id="landing-page" class="md:h-screen mb-10">
        <Navbar />
        <Splash />
        <div
          id="splash-footer"
          class="flex justify-between items-center w-full"
        >
          <div id="line"></div>
          <div class="flex ml-2">
            <a href="https://github.com/acaala">
              <IconsGithub class="mr-12"
            /></a>
            <a href="https://www.linkedin.com/in/lawatts1/"
              ><IconsLinkedin
            /></a>
          </div>
        </div>
      </div>

      <!-- Projects -->
      <div id="projects" class="grid grid-cols-1 my-5">
        <Project />
        <FeaturedProject />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import { defineComponent, onMounted, ref } from '@nuxtjs/composition-api'
export default defineComponent({
  setup() {
    const didLoad = ref(false)
    onMounted(() => {
      const t3 = gsap.timeline()

      t3.from('#splash-footer', { duration: 3, x: -300, opacity: 0 })

      didLoad.value = true
    })
  },
})
</script>

<style lang="postcss" scoped>
#line {
  height: 1px;
  @apply w-3/4 bg-gray-200;
}
</style>

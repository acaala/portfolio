<template>
  <div class="flex items-center justify-center md:justify-between my-32 p-x-4">
    <div id="hero-content" class="text-center md:text-left">
      <h1 class="uppercase text-5xl font-medium primary-color">
        Creating Unique <br />Experiences
      </h1>
      <div class="flex mt-5 items-center justify-center md:justify-start">
        <Scroll />
        <p class="tracking-widest text-sm font-medium uppercase px-5">
          Scroll for more!
        </p>
      </div>
    </div>
    <HeroImg class="hidden md:block" />
  </div>
</template>

<script>
import { defineComponent, onMounted } from '@nuxtjs/composition-api'

export default defineComponent({
  setup() {
    onMounted(() => {
      const t1 = gsap.timeline()

      t1.from('#hero-content', { duration: 3, x: -300, opacity: 0 })
    })
  },
})
</script>

<style lang="postcss" scoped>
p {
  color: #b4fee7;
}
</style>
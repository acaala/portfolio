<template>
  <div class="container mx-auto px-2 h-full">
    <Navbar />
    <Splash />
    <div class="flex justify-between items-center w-full">
      <div id="line"></div>
      <div class="flex ml-2">
        <a href="https://github.com/acaala"> <Github class="mr-12" /></a>
        <a href="https://www.linkedin.com/in/lawatts1/"><Linkedin /></a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'

export default defineComponent({
  setup() {},
})
</script>

<style lang="postcss" scoped>
#line {
  height: 1px;
  @apply w-3/4 bg-gray-200;
}
</style>

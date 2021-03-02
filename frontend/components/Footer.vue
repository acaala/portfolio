<template>
  <footer>
    <h1 class="text-xl">Want to know more?</h1>
    <nuxt-link to="/contact"
      ><button class="btn-primary">Let's Talk</button></nuxt-link
    >
  </footer>
</template>

<script>
export default {}
</script>

<style lang="postcss">
h1 {
  color: #4cfcd3;
}
footer {
  background-color: #32145a;
  border-top-right-radius: 100px;
  @apply mr-10 flex justify-around items-center py-12;
}
</style>
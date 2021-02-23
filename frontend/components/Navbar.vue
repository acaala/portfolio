<template>
  <header class="flex justify-between primary-color items-center my-4">
    <div class="w-2/3 flex justify-between items-center">
      <div>
        <h1 class="title-font text-3xl">Liam Watts</h1>
      </div>
      <div class="hidden md:flex">
        <a href="#">My work</a>
        <a href="#projects">projects</a>
      </div>
    </div>

    <div>
      <button>Let's Talk</button>
    </div>
  </header>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
a {
  @apply tracking-widest text-sm font-medium uppercase px-5;
}
</style>
<template>
  <header class="flex justify-between primary-color items-center my-4">
    <div class="w-2/3 flex justify-between items-center">
      <div>
        <h1 class="title-font text-3xl">Liam Watts</h1>
      </div>
      <div class="hidden md:flex">
        <a href="#projects">projects</a>
      </div>
    </div>

    <div>
      <nuxt-link to="/contact">
        <button class="btn-primary">Let's Talk</button>
      </nuxt-link>
    </div>
  </header>
</template>

<style lang="postcss" scoped>
a {
  @apply tracking-widest text-sm font-medium uppercase px-5;
}
</style>
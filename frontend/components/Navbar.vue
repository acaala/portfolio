<template>
  <header class="flex justify-between primary-color items-center mt-2">
    <div class="w-2/3 flex justify-between items-center">
      <div>
        <h1 class="title-font text-3xl">Liam Watts</h1>
      </div>
      <div>
        <a href="#">My work</a>
        <a href="#">My projects</a>
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
button {
  background-color: #ff45b5;
  color: #ffffff;
  @apply px-5 py-1 rounded-full;
}
button:hover {
  background-color: #ffffff;
  color: #ff45b5;
}
</style>
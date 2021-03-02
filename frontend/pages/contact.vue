<template>
  <div class="container mx-auto">
    <header class="flex justify-between mx-auto items-center py-4">
      <h1 class="title-font text-3xl primary-color">Liam Watts</h1>
      <nuxt-link to="/">
        <button class="btn-secondary">close</button>
      </nuxt-link>
    </header>

    <section class="my-12 container mx-auto">
      <h2 class="title-font text-3xl text-center text-white">Hi, Let's Talk</h2>

      <form
        class="flex flex-col container lg:w-1/2 md:w-2/3 mx-auto space-y-20 my-12"
      >
        <div class="flex flex-col">
          <label for="name" class="">Name</label>
          <input type="text" name="name" required />
        </div>
        <div class="flex flex-col">
          <label for="email">Email</label>
          <input type="email" name="email" required />
        </div>
        <div class="flex flex-col">
          <label for="message">Message</label>
          <textarea
            name="message"
            id="message"
            cols="30"
            rows="5"
            required
          ></textarea>
        </div>
        <div class="w-1/3 mx-auto">
          <button class="btn-primary w-full">Send</button>
        </div>
      </form>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style lang="postcss" scoped>
label {
  @apply leading-7 text-sm text-gray-400;
}

input,
textarea {
  outline: none;
  background: unset;
  border-bottom: 1px solid #4cfcd3;
  color: white;
  @apply px-3 rounded-sm py-1  transition-colors duration-200 ease-in-out;
}

input:focus,
textarea:focus {
  background-color: #a16ae8;
}
</style>>

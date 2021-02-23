<template>
  <div>
    <Nuxt />
    <Footer />
  </div>
</template>

<style lang="postcss">
html {
  font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #7b3ccc;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.primary-bg {
  background-color: #7b3ccc;
}

.primary-color {
  color: #4cfcd3;
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

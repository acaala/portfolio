<template>
  <div>
    <Nuxt />
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

.btn-primary {
  border: 1px solid #ff45b5;
  background-color: #ff45b5;
  color: #ffffff;
  @apply px-5 py-1 rounded-full;
}
.btn-primary:hover {
  background-color: #ffffff;
  color: #ff45b5;
}

.btn-secondary {
  border: 1px solid #c53030;
  color: #ffffff;
  @apply px-5 py-1 rounded-full;
}
.btn-secondary:hover {
  background-color: #c53030;
}

.btn-project-card {
  border: 1px solid #7b3ccc;
  color: #7b3ccc;
  @apply px-5 py-1 rounded-full;
}

.btn-project-card:hover {
  background-color: #7b3ccc;
  color: #ffffff;
}
</style>

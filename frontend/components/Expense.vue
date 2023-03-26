<template>
    <div
      id="featured-project"
      class="container bg-white rounded-xl lg:flex items-center px-5 py-10"
    >
      <!-- Text content -->
      <div
        id="featured-text"
        class="
          lg:w-1/3
          mx-auto
          text-center
          lg:text-left
          lg:mx-4
          px-2
          mb-2
          md:mb-0
          py-2
        "
      >
        <h3 class="uppercase tracking-widest text-xs lg:text-sm font-medium">
          Under Construction
        </h3>
  
        <h2 class="uppercase text-2xl xl:text-3xl font-medium">
          Expense <small>(Name TBD)</small>
        </h2>
  
        <p class="leading-relaxed text-gray-900 my-4">
          Full stack Symfony app, empowering business to manage expenses with ease.
        </p>
        <div
          class="
            flex
            lg:flex-col
            space-x-10
            lg:space-y-4 lg:space-x-0
            justify-center
            text-center
            my-4
          "
        >
          <!-- <a href="" disabled class="btn-primary"
            >Under Construction</a
          > -->
          <!-- <a
            href="https://github.com/acaala/url-shortener"
            class="btn-project-card"
            >Github Repo</a
          > -->
        </div>
      </div>
      <!-- Picture -->
      <div id="project-image" class="md:w-2/3 lg:ml-5 shadow-md">
        <img src="../static/expense.png" alt="Url image" class="w-full rounded-3xl" />
      </div>
    </div>
  </template>
  
  
  <style lang="postcss" scoped>
  h3 {
    color: #fd49a0;
  }
  
  #project-image {
    background: #4cfcd3;
    @apply rounded-3xl pt-2 w-full pr-2;
  }
  </style>
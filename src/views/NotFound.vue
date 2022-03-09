<template>
  <div
    class="w-9/12 m-auto py-16 min-h-screen flex items-center justify-center"
  >
    <div class="bg-white shadow overflow-hidden sm:rounded-lg pb-8">
      <div class="border-t border-gray-200 text-center pt-8">
        <h1 class="text-9xl font-bold text-purple-400">404</h1>
        <h1 class="text-6xl font-medium py-8">oops! Page not found</h1>
        <p class="text-2xl pb-8 px-12 font-medium">
          Oops! The page you are looking for does not exist. It might have been
          moved or deleted.
        </p>
        <router-link
          to="/dashboard"
          class="bg-gradient-to-r from-purple-400 to-blue-500 hover:from-pink-500 hover:to-orange-500 text-white font-semibold px-6 py-2 rounded-md mr-6"
        >
          HOME
        </router-link>
        <router-link
          to="/"
          class="bg-gradient-to-r from-red-400 to-red-500 hover:from-red-500 hover:to-red-500 text-white font-semibold px-6 py-2 rounded-md"
        >
          Contact Us
        </router-link>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style>
.text-9xl {
  font-size: 14rem;
}
@media (max-width: 645px) {
  .text-9xl {
    font-size: 5.75rem;
  }
  .text-6xl {
    font-size: 1.75rem;
  }
  .text-2xl {
    font-size: 1rem;
    line-height: 1.2rem;
  }
  .py-8 {
    padding-top: 1rem;
    padding-bottom: 1rem;
  }
  .px-6 {
    padding-left: 1.2rem;
    padding-right: 1.2rem;
  }
  .mr-6 {
    margin-right: 0.5rem;
  }
  .px-12 {
    padding-left: 1rem;
    padding-right: 1rem;
  }
}
</style>

<template>
  <div class="h-screen bg-blue-50 flex flex-col justify-center items-center">
    <img src="@/assets/svg/404.svg" alt="404" />
    <h1 class="my-4 text-2xl md:text-4xl font-extrabold text-gray-800 capitalize">
      Back to home page!
    </h1>
    <NuxtLink
      to="/"
      class="
        bg-indigo-500
        hover:bg-indigo-600
        shadow-lg
        px-16
        py-2
        md:py-4
        rounded-full
        text-white
        text-2xl
        md:text-4xl
      "
    >
      &larr; Back
    </NuxtLink>
  </div>
</template>

<script>
export default {
  layout: "blankLayout",
};
</script>

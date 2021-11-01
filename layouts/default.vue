<template>
  <div class="bg-blue-50 bg-opacity-50">
    <Header />
    <div class="h-withoutHeader flex">
      <SideBar :class="{ 'w-0': toggleSideBar, 'w-80': !toggleSideBar }" />
      <div class="w-full p-6 overflow-y-auto">
        <div class="py-2 ">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            width="24"
            height="24"
            class="cursor-pointer"
            :class="{ 'transform rotate-180': toggleSideBar }"
            @click="toggleSideBar = !toggleSideBar"
          >
            <path fill="none" d="M0 0h24v24H0z" />
            <path
              d="M7.828 11H20v2H7.828l5.364 5.364-1.414 1.414L4 12l7.778-7.778 1.414 1.414z"
            />
          </svg>
        </div>
        <Nuxt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggleSideBar: false,
    };
  },
};
</script>

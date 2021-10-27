<template>
  <div class="overflow-hidden">
    <!-- MenuItem -->
    <div class="menuItem" @click="itemOpen = !itemOpen">
      <span class="mr-2">
        <slot name="icon"></slot>
      </span>
      <p>{{ label }}</p>
      <span
        v-if="arrow"
        class="arrow"
        :class="{ 'transform rotate-90': itemOpen }"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          width="24"
          height="24"
        >
          <path fill="none" d="M0 0h24v24H0z" />
          <path
            d="M12.172 12L9.343 9.172l1.414-1.415L15 12l-4.243 4.243-1.414-1.415z"
          />
        </svg>
      </span>
    </div>

    <!-- MenuItem Child -->
    <div
      class="menuItemChildWrapper max-h-0"
      :class="{ 'max-h-screen': itemOpen }"
    >
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ["icon", "label", "arrow"],
  data() {
    return {
      itemOpen: false,
    };
  },
};
</script>

<style scoped>
.menuItem {
  @apply flex items-center p-2 font-bold text-gray-800;
  @apply hover:bg-blue-50;
}

.arrow {
  @apply ml-auto transition-all duration-500;
}

.menuItemChildWrapper {
  @apply pl-4 divide-y divide-gray-100 transition-all duration-500 ease-in-out;
}
</style>

<template>
  <div class="menuItemChild">
    <slot></slot>
  </div>
</template>

<style scoped>
.menuItemChild {
  @apply p-2 text-gray-600;
  @apply hover:bg-blue-50;
}
</style>

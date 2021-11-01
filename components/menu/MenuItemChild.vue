<template>
  <div class="menuItemChild" @click="$router.push({ name: pageName })">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ["pageName"],
};
</script>

<style scoped>
.menuItemChild {
  @apply p-2 text-gray-600;
  @apply hover:bg-blue-50;
}
</style>

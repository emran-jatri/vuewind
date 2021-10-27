<template>
  <div class="bg-white w-80 overflow-y-auto">
    <Menu>
      <MenuItem icon={ToggleOutlineSvg} label="Components" :arrow="true">
        <template v-slot:icon>
          <ToggleOutlineSvg />
        </template>
        <MenuItemChild>Button</MenuItemChild>
        <MenuItemChild>Modal</MenuItemChild>
        <MenuItemChild>Card</MenuItemChild>
      </MenuItem>
      <MenuItem label="Components" :arrow="true">
        <template v-slot:icon>
          <!-- <FontAwesomeIcon :icon="['fab', 'facebook-f']" /> -->
        </template>
        <MenuItemChild>Button</MenuItemChild>
        <MenuItemChild>Modal</MenuItemChild>
        <MenuItemChild>Card</MenuItemChild>
      </MenuItem>
      <MenuItem label="Components" :arrow="true">
        <MenuItemChild>Button</MenuItemChild>
        <MenuItemChild>Modal</MenuItemChild>
        <MenuItemChild>Card</MenuItemChild>
      </MenuItem>
    </Menu>
  </div>
</template>

<script>
export default {};
</script>

<style></style>

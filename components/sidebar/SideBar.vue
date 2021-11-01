<template>
  <div class="bg-white overflow-y-auto transition-all duration-500 ease-in-out">
    <Menu>
      <MenuItem icon="{ToggleOutlineSvg}" label="Components" :arrow="true">
        <template v-slot:icon>
          <ToggleOutlineSvg />
        </template>
        <MenuItemChild pageName="components-button">Button</MenuItemChild>
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

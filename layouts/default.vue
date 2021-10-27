<template>
  <div class="bg-blue-50">
    <Header />
    <div class="h-withoutHeader flex">
      <SideBar />
      <div class="w-full p-6 overflow-y-auto">
        <div>
          <Nuxt />
        </div>
      </div>
    </div>
  </div>
</template>

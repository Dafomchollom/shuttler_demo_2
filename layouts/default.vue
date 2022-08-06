<template>
  <div class="bg-white h-screen w-screen flex gap-x-2">
    <div class="sidebar cols-span-1 w-20 h-full">
      <app-side-bar-component />
    </div>
    <div class="main cols-span-11 w-full h-full py-5 px-3">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {
  components: {
    AppNavbarComponent: () =>
      import("@/components/layout/AppNavbarComponent.vue"),
    AppSideBarComponent: () =>
      import("@/components/layout/AppSideBarComponent.vue"),
  },
};
</script>

<style></style>

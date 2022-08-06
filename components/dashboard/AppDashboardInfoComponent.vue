<template>
  <div class="grid grid-cols-12">
    <div class="cols-span-4">
      <!-- active user component -->
      <app-active-users-component />
    </div>
    <div class="cols-span-8"></div>
  </div>
</template>

<script>
import AppActiveUsersComponent from "@/components/dashboard/AppActiveUsersComponent.vue";
export default {
  name: "AppActiveUsersComponent",
  components: {
    AppActiveUsersComponent
    // AppActiveUsersComponent: () =>
    //   import(""),
  },
};
</script>

<style></style>

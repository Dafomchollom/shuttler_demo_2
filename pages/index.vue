<template>
  <div class="">
    <AppWelcomeComponent />
    <hr />
    <div class="w-full grid grid-cols-12 mt-5 gap-x-5">
      <div class="col-span-3">
        <!-- active user component -->
        <AppActiveUsersComponent />
      </div>
      <div class="col-span-9">
        <AppMonthlySpendingComponent />
      </div>
    </div>
  </div>
</template>

<script>
import AppActiveUsersComponent from "@/components/dashboard/AppActiveUsersComponent.vue";

import AppMonthlySpendingComponent from "@/components/dashboard/AppMonthlySpendingComponent.vue";
export default {
  name: "IndexPage",
  components: {
    AppWelcomeComponent: () =>
      import("@/components/dashboard/AppWelcomeComponent.vue"),
    AppActiveUsersComponent,
    AppMonthlySpendingComponent,
    // AppDashboardInfoComponent,
    // AppDashboardInfoComponent: () =>
    // import("@/components/dashboard/AppDashboardInfoComponent.vue"),
  },
};
</script>

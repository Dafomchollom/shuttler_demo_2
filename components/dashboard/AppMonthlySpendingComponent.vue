<template>
  <div class="rounded border border-gray-200 shadow-md py-5">
    <div class="flex justify-between px-5">
      <h3>Monthly spending</h3>
      <div>
        <AppButtonGroupToggler
          v-model="currentFilter"
          :filterItems="filterList"
        />
      </div>
    </div>
  </div>
</template>

<script>
import AppButtonGroupToggler from "@/components/input/AppButtonGroupToggler.vue";
export default {
  name: "AppMonthlySpendingComponent",
  components: {
    AppButtonGroupToggler,
  },
  data() {
    return {
      currentFilter: "",
      filterList: ["this month", "last month", "custom"],
    };
  },
};
</script>

<style></style>

<template>
  <div class="w-full rounded border border-gray-200 shadow-md py-7 px-5">
    <div class="w-full flex justify-between">
      <h2 class="font-medium">Active users right now</h2>
      <button>
        <img
          src="@/assets/images/icons/moreIcon.svg"
          width="5"
          height="5"
          alt=""
        />
      </button>
    </div>
    <div>
      <h1 class="font-bold text-3xl py-3">10.8k</h1>
      <div>
        <div
          v-for="(user, index) in usersData"
          :key="index"
          class="flex w-full gap-x-3 items-start my-3"
        >
          <img class="w-8" :src="user.flagPath" alt="" />
          <div class="w-full">
            <p class="mb-3">United States</p>
            <AppProgressBarComponent :progress="50" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppProgressBarComponent from "@/components/dashboard/AppProgressBarComponent.vue";
export default {
  components: {
    AppProgressBarComponent,
  },
  data() {
    return {
      usersData: [
        { country: "USA", flagPath: require("assets/images/icons/US.svg") },
        { country: "INDIA", flagPath: require("assets/images/icons/IN.svg") },
        { country: "INDIA", flagPath: require("assets/images/icons/GB.svg") },
      ],
    };
  },
};
</script>

<style></style>

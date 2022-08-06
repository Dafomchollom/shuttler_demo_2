<template>
  <div class="bg-purple-700 h-full w-full py-3">
    <div class="brand flex justify-center w-full py-3">
      <img src="@/assets/images/icons/Logomark.svg" width="50" alt="" />
    </div>
    <div class="">
      <a
        v-for="(items, index) in sidebar"
        :key="index"
        class="flex justify-center w-full py-4"
      >
        <img :src="items.iconPath" width="30" alt="" />
      </a>
      <!-- <a class="flex justify-center w-full py-4">
        <img src="@/assets/images/icons/home.svg" width="30" alt="" />
      </a>
      <a class="flex justify-center w-full py-4">
        <img src="@/assets/images/icons/alarm.svg" width="30" alt="" />
      </a>
      <a class="flex justify-center w-full py-4">
        <img src="@/assets/images/icons/layers.svg" width="30" alt="" />
      </a> -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sidebar: [
        {
          name: "Home",
          iconPath: require("@/assets/images/icons/home.svg"),
        },
        {
          name: "Notifications",
          iconPath: require("@/assets/images/icons/alarm.svg"),
        },
        {
          name: "Home",
          iconPath: require("@/assets/images/icons/layers.svg"),
        },
        {
          name: "Home",
          iconPath: require("@/assets/images/icons/Logomark.svg"),
        },
      ],
    };
  },
};
</script>

<style></style>

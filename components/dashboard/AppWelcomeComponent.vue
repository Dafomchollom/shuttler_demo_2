<template>
  <div class="w-full justify-between flex pt-5 pb-10">
    <div class="">
      <h1 class="text-black text-4xl mb-1">Your Cards</h1>
      <p class="text-gray-400 text-xl font-xs">Welcome back olivia</p>
    </div>
    <div class="lg:flex justify-between gap-x-4">
      <button
        class="border border-1 border-gray-200 h-10 px-4 rounded-lg shadow-md flex gap-x-3 items-center"
      >
        <img src="@/assets/images/icons/sync.svg" alt="" />
        Sync Accounts
      </button>
      <button class="bg-purple-700 h-10 px-4 rounded-lg text-white shadow-md">
        Add Card
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppWelcomeComponent",
};
</script>

<style></style>

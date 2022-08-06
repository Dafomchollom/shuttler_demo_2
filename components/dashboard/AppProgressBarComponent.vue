<template>
  <div class="flex gap-x-3">
    <div class="w-full bg-gray-200 h-2 rounded-xl">
      <div
        class="bg-purple-700 h-2 rounded-xl"
        :style="`width: ${progress}%;`"
      ></div>
    </div>
    <span>{{ progress }}%</span>
  </div>
</template>

<script>
export default {
  name: "AppProgressBarComponent",
  props: {
    progress: {
      type: Number,
      default: 0,
      required: true,
    },
  },
};
</script>

<style></style>

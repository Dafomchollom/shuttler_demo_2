<template>
  <div class="flex">
    <button
      v-for="(item, index) in filterItems"
      :key="index"
      class="border border-gray-200 px-5 py-2"
      :class="{
        'bg-gray-200': value === item,
        'rounded-tl-lg rounded-bl-lg': index === 0,
      }"
      @click="filterTogglerHandler(item)"
    >
      {{ item }}
    </button>
  </div>
</template>

<script>
export default {
  name: "AppButtonGroupToggler",
  props: {
    filterItems: {
      type: "Array",
      default: () => [],
    },
    value: {
      type: String,
      default: "",
    },
  },
  methods: {
    filterTogglerHandler(filter) {
      this.$emit("input", filter);
    },
  },
};
</script>

<style></style>

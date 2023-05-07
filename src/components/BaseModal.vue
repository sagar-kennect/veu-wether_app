<template>
  <div v-if="modalActive">
    <div class="p-4 bg-white self-start mt-32 max-w-screen-md">
      <slot />
      <button class="text-white mt-8 bg-weather-primary py-2 px-6">
        Close
      </button>
    </div>
  </div>
</template>

<script setup>
defineProps({
  modalActive: {
    type: Boolean,
    default: false,
  },
});
</script>

<style lang="scss" scoped></style>

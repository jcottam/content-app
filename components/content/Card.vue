<script setup>
defineProps({
  type: {
    type: String,
    required: false,
  },
});
</script>

<template>
  <div
    :class="[type]"
    class="p-2 border bg-white dark:bg-black dark:border-gray-700 rounded"
  >
    <!-- <Icon name="uil:github" class="h-4 w-4" /> -->
    Type: {{ type }}
    <slot />
  </div>
</template>

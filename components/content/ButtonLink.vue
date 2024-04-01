<script setup>
defineProps({
  href: {
    type: String,
    required: true,
  },
  external: {
    type: Boolean,
    default: false,
  },
  icon: {
    type: String,
    default: "",
  },
});
</script>

<template>
  <NuxtLink :to="href" target="_blank" rel="noopener">
    <button>
      <!-- <Icon name="uil:github" class="h-4 w-4" /> -->
      <!-- <Icon :name="icon" class="w-4 h-4" /> -->
      {{ icon }}
    </button>
  </NuxtLink>
</template>

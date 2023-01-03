<script setup lang="ts">
const props = defineProps<{
  type: "warning" | "info" | "error";
}>();
</script>

<template>
  <div>
    <slot />
  </div>
</template>

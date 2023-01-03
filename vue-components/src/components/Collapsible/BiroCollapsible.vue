<script setup lang="ts">
const props = defineProps<{
  title?: string;
}>();
</script>

<template>
  <div>
    <h2>{{ props.title }}</h2>
    <div id="contents">
      <slot />
    </div>
  </div>
</template>

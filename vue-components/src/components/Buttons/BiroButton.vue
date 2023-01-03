<script setup lang="ts">
import { StyleValue } from "vue";

const props = defineProps<{
  title?: string;
  className?: string;
  onClick?: () => void;
  readonly rounded?: boolean;
  readonly circle?: boolean;
  thiccness?: 0.5 | 1 | 2 | 3 | 4 | 5;
  style?: StyleValue;
}>();
</script>

<template>
  <button @click="props.onClick" :title="props.title" :style="style">
    <slot />
  </button>
</template>

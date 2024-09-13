<script setup lang="ts">
import { computed } from "vue";
const { page } = defineProps<{ page: number }>();
const TOTAL_PAGES = 51;
const pageRatio = computed(() => `${page} / ${TOTAL_PAGES}`);
</script>

<template>
  <div class="abs-br m-6 first-letter:text-green">
    {{ pageRatio }}
  </div>
</template>

<script setup lang="ts">
import BentoGrid from "@bentogrid/core";

onMounted(() => {
  new BentoGrid({
    cellGap: 12,
    columns: 2,
    breakpoints: {
      640: {
        columns: 4,
        cellGap: 18
      }
    }
  });
})
</script>

<template>
  <div class="bentogrid">
    <slot></slot>
  </div>
</template>

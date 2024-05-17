<script setup lang="ts">
defineProps({
  size: {
    type: String,
    required: true
  }
});
</script>

<template>

  <div :data-bento="size" class="bento">
    <div class="content">
      <slot></slot>
    </div>
  </div>
</template>

<style scoped lang="scss">
.bento {
  background-color: hsl(0, 0%, 96%);
  border: 2px solid hsl(0, 0%, 92%);
  border-radius: 24px;

  &>.content {
    height: 100%;
    padding: 15px;
  }
}
</style>

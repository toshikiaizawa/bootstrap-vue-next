<template>
  <div class="bl_modal_header">
    {{ props.title }}
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'
const props = defineProps({
  title: { type: String, default: 'モーダルタイトル' },
})
</script>

<style scoped>
.bl_modal_header {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
}
</style>

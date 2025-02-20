<script setup lang="ts">
import { ref } from 'vue';
import Modal from '@/components/Modal.vue';

const modal = ref(false);
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="modal = !modal">押すとモーダルが表示できる</button>
  </div>
  <Modal v-model="modal"></Modal>
</template>

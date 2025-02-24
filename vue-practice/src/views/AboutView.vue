<script setup lang="ts">
import { ref } from 'vue'
import Modal from '@/components/Modal.vue'
import CustomModal from '@/components/Modal/CustomModal.vue'

const modal = ref(false)
const isOpen = ref(true)
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="modal = !modal">押すとモーダルが表示できる</button>
    <button @click="isOpen = !isOpen">押すとカスタムモーダルが表示できる</button>
  </div>
  <Modal v-model="modal"></Modal>
  <CustomModal v-model="isOpen">
    <template #footer></template>
  </CustomModal>
</template>

<template>
  <BModal no-footer>
    <div class="modal-footer d-flex justify-content-end">
      <slot name="footer">
        <ModalFooter></ModalFooter>
      </slot>
    </div>
  </BModal>
</template>

<script setup lang="ts">
import { BModal } from 'bootstrap-vue-next'
import ModalFooter from './ModalFooter.vue'
</script>

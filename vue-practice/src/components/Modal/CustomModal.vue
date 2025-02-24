<template>
  <BModal no-footer>
    <div class="modal-footer">
      <ModalFooter>
        <slot name="footer"> </slot>
      </ModalFooter>
    </div>
  </BModal>
</template>

<script setup lang="ts">
import { BModal } from 'bootstrap-vue-next'
import ModalFooter from './ModalFooter.vue'
</script>

<style>
.modal-footer {
  padding: 0;
}
</style>

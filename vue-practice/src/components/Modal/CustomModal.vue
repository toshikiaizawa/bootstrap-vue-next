<template>
  <BModal no-header no-footer>
    <div class="modal-header">
      <ModalHeader>
        <slot name="header"></slot>
      </ModalHeader>
    </div>
    <div class="modal-body">
      <ModalBody>
        <slot name="body"></slot>
      </ModalBody>
    </div>
    <div class="modal-footer">
      <ModalFooter>
        <slot name="footer"> </slot>
      </ModalFooter>
    </div>
  </BModal>
</template>

<script setup lang="ts">
import { BModal } from 'bootstrap-vue-next'
import ModalHeader from './ModalHeader.vue'
import ModalBody from './ModalBody.vue'
import ModalFooter from './ModalFooter.vue'
</script>

<style>
.modal-footer {
  padding: 0;
}
.modal-header {
  padding: 0;
}
</style>

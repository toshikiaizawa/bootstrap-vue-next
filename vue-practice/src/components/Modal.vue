<template>
  <BButton @click="$emit('update:modelValue', !modelValue)">Toggle modal</BButton>
  <BModal :model-value="modelValue" title="Hello, World!" @hide="$emit('update:modelValue', false)">
    Foobar?
  </BModal>
</template>

<script setup lang="ts">
import { BModal } from 'bootstrap-vue-next';
import { defineProps, defineEmits } from 'vue';

defineProps<{ modelValue: boolean }>();
defineEmits(['update:modelValue']);
</script>

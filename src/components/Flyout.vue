<template>
  <div class="flyout">
    <button class="close" @click="$emit('close')">CLOSE</button>
    <contact-form />
  </div>
</template>

<script setup>
import ContactForm from './ContactForm.vue'

defineProps({
  isOpen: Boolean,
});

defineEmits(['close']);
</script>

<style>
.flyout {
  background-color: black;
  min-height: 100vh;
  position: absolute;
  top: 0;
  width: 50%;
}

.close {
  display: flex;
  margin-left: auto;
}
</style>

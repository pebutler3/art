<template>
  Flyout
  {{ isOpen || 'not open' }}
</template>

<script setup>

defineProps({
  isOpen: Boolean,
});
</script>

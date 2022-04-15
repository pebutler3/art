<template>
  <nav>
    <ul>
      <li>
        <button @click="$emit('toggleFlyout')">
          Contact
        </button>
      </li>
    </ul>
  </nav>
</template>

<script setup>
defineEmits([
  'toggleFlyout'
])
</script>

<style>
ul {
  display: flex;
  background-color: black;
  list-style: none;
  margin: 0;
  padding: 0;
}

li {
  margin-left: auto;
  padding: 0.5rem 0;
}

button {
  background-color: white;
  border: none;
  padding: 1rem 2rem;
}
</style>

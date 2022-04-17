<template>
  <div class="overlay" v-if="flyout.isOpen" />
  <Navigation @toggle-flyout="toggleFlyout" />
  <Flyout :isOpen="flyout.isOpen" v-if="flyout.isOpen" @close="toggleFlyout" />
  <main>
    <Bio />
    <Gallery />
  </main>
</template>

<script setup>
import { reactive } from 'vue';
import Bio from './components/Bio.vue';
import Gallery from './components/Gallery.vue';
import Navigation from './components/Navigation.vue';
import Flyout from './components/Flyout.vue';

const flyout = reactive({
  isOpen: false
});

const toggleFlyout = () => flyout.isOpen = !flyout.isOpen;
</script>

<style>
html,
body {
  height: 100%;
}

body {
  padding: 0;
  margin: 0;
}

#app {
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  position: relative;
}

.overlay {
  background-color: #1b0a20;
  height: 100vh;
  max-width: 100%;
  opacity: 0.95;
  position: absolute;
  width: 100%;
}

main {
  background: url('/doodle.jpeg') no-repeat center;
  background-size: cover;
  display: flex;
  min-height: 100vh;
  padding: 0 2rem;
  gap: 10px;
}

h1,
h2,
p {
  background-color: black;
  color: white;
  padding: 1rem 0.5rem;
  margin-bottom: 0;
}

button {
  cursor: pointer;
}
</style>


<template>
  <Navigation />
  <button @click="openFlyout">open flyout</button>
  <Flyout :isOpen="flyoutOpen"/>
  <main>
    <Bio></Bio>
  </main>
</template>

<script setup>
import Bio from './components/Bio.vue'
import Navigation from './components/Navigation.vue'
import Flyout from './components/Flyout.vue'

let flyoutOpen = false;

const openFlyout = () => {
  return flyoutOpen = !flyoutOpen;
}
</script>

<style>
body {
  padding: 0;
  margin: 0;
}

#app {
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

main {
  padding: 0 2rem;
}
</style>


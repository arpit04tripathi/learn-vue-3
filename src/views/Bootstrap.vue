<template>
  <div>
      <h1>This is bootstrap view</h1>
      <MyBootstrapIcons />
  </div>
</template>

<script setup lang="ts">
import MyBootstrapIcons from '../components/test/MyBootstrapIcons.vue'
</script>

<style>
@media (min-width: 1024px) {
.about {
  min-height: 100vh;
  display: flex;
  align-items: center;
}
}
</style>

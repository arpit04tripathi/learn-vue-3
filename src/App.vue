<script setup lang="ts">
import { RouterView } from 'vue-router'
import HeaderComponent from '@/components/_layout/HeaderComponent.vue';
import FooterComponent from '@/components/_layout/FooterComponent.vue';
</script>

<template>
  <div class="flex-wrapper">
    <HeaderComponent />
    <main class="container-fluid my-3 p-3 brdr">
      <RouterView />
    </main>
    <FooterComponent class="mt-auto p-3 brdr" />
  </div>
</template>

<style scoped>
.flex-wrapper {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
  justify-content: space-between;
}

.brdr {
  border: dashed red 1px;
}
</style>

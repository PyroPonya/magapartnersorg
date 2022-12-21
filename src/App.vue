<template>
  <div class="app_container">
    <WelcomePage />
  </div>
</template>

<script setup>
import WelcomePage from './views/WelcomePage.vue';
</script>

<style scoped>
* {
  font-family: 'Montserrat', sans-serif;
  font-style: normal;
}
.app_container {
  background-color: #f1f0f1;
  width: 100%;
  display: flex;
  justify-content: flex-start;
}
</style>

<template>
  <div class="view_container">
    <ComponentHeader />
    <ComponentWelcome />
  </div>
</template>

<script setup>
import ComponentHeader from '../components/ComponentHeader.vue';
import ComponentWelcome from '../components/ComponentWelcome.vue';
</script>

<style scoped>
.view_container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 50px 100px;
  min-height: 100vh;
  max-width: 100vw;
  margin: 0 auto;
}
/* @media (min-width: 1024px) {
  .app_container {
    display: flex;
  }
} */
</style>

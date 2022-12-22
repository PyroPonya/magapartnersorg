<template>
  <div class="view_container">
    <ComponentHeader />
    <ComponentWelcome />
    <ComponentAboutus />
    <ComponentPartners />
  </div>
</template>

<script setup>
import ComponentHeader from '../components/ComponentHeader.vue';
import ComponentWelcome from '../components/ComponentWelcome.vue';
import ComponentAboutus from '../components/ComponentAboutus.vue';
import ComponentPartners from '../components/ComponentPartners.vue';
setTimeout(() => {
  alert(`
  Merry Christmas and Happy New Year!
  The site is currently under construction.
  It will look much better soon!`);
}, 5000);
</script>

<style scoped>
.view_container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  /* padding: 50px 100px; */
  padding: 50px 0px;
  min-height: 100vh;
  /* max-width: 100vw; */
  margin: 0 auto;
  /* max-width: 1700px; */
  max-width: 1500px;
  background-color: #f1f0f1;
}
@media (min-width: 1400px) {
  .view_container {
    /* padding: 5px 10px; */
  }
}
</style>

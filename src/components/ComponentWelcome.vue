<template>
  <div class="welcome_container">
    <div class="slider">
      <ComponentWelcomeSwiper />
    </div>
    <div class="information_section">
      <div class="section_title">information</div>
      <div class="section_list">
        <div v-for="(el, id) in listText" :key="id" class="list_element">
          <div class="element_title">
            {{ el.title }}
          </div>
          <div class="element_content">
            {{ el.content }}
          </div>
        </div>
      </div>
      <!-- <a href="https://backoffice.megapartners.org/partner/register">
        <div class="section_btn">become&nbsp;a&nbsp;partner</div>
      </a> -->
    </div>
  </div>
</template>

<script setup>
import ComponentWelcomeSwiper from './ComponentWelcomeSwiper.vue';
const listText = [
  {
    title: 'Meet us at Malta Sigma 2022',
    content:
      'From September 14 to 18, the Megapartners.io will be hosting the largest bar area at the conference...',
  },
  {
    title: 'Meet us at Malta Sigma 2022',
    content:
      'From September 14 to 18, the Megapartners.io will be hosting the largest bar area at the conference...',
  },
  {
    title: 'Meet us at Malta Sigma 2022',
    content:
      'From September 14 to 18, the Megapartners.io will be hosting the largest bar area at the conference...',
  },
  {
    title: 'Meet us at Malta Sigma 2022',
    content:
      'From September 14 to 18, the Megapartners.io will be hosting the largest bar area at the conference...',
  },
  {
    title: 'Meet us at Malta Sigma 2022',
    content:
      'From September 14 to 18, the Megapartners.io will be hosting the largest bar area at the conference...',
  },
];
</script>

<style scoped>
.welcome_container {
  width: 100%;
  display: grid;
  grid-template-columns: 3fr 1fr;
  gap: 1rem;
  padding-bottom: 2rem;
  margin-bottom: 2rem;
}
.slider {
  min-width: 300px;
  min-width: 100%;
  max-width: 100%;
  height: 554px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.information_section {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: flex-start;
  gap: 26px;
}
.section_title {
  width: 420px;
  height: 130px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #ffffff;
  border: 1px solid #282841;
  font-family: 'Oranienbaum', serif;
  font-style: normal;
  font-weight: 400;
  font-size: 60px;
  line-height: 69px;
  display: flex;
  align-items: center;
  text-transform: uppercase;
  color: #282841;
}
.section_list {
  overflow-y: scroll;
  width: 420px;
  height: 400px;
  padding: 44px 36px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  border: 1px solid #282841;
}
.section_list::-webkit-scrollbar {
  width: 5px;
}

.section_list::-webkit-scrollbar-track {
  background-color: none;
}

.section_list::-webkit-scrollbar-thumb {
  box-shadow: inset 0px 0px 10px #282841;
}
.list_element {
  padding-bottom: 36px;
  /* margin-bottom: 36px; */
  border-bottom: 1px solid #282841;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  gap: 15px;
}
.list_element:not(:first-of-type) {
  margin-top: 36px;
}
.element_title {
  font-weight: 600;
  font-size: 30px;
  line-height: 37px;
  color: #4790fe;
}
.element_content {
  font-weight: 300;
  font-size: 16px;
  line-height: 20px;
  color: #282841;
}
/* .section_btn {
  background-color: #4790fe;
  height: 50px;
  width: 220px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
  color: #282841;
  text-transform: uppercase;
  border: 1px solid #4790fe;
}
.section_btn:hover {
  background-color: #ffffff;
  border-color: #282841;
} */
</style>

<template>
  <div class="partners_container">
    <div class="partners_header">Partners</div>
    <div class="partners_list">
      <div
        v-for="(el, id) in partnerList"
        :key="id"
        class="list_element-container"
      >
        <div class="list_element">
          <div
            :style="`--hover_img_partners: url(${el.logo}); --img_partners: url(${el.logo_dark})`"
            class="element_logo"
          ></div>
          <div class="element_head">
            {{ el.head }}
          </div>
          <a :href="'https://www.' + el.link">
            <div class="element_link">
              {{ el.link }}
            </div>
          </a>
          <div class="element_body">
            {{ el.body }}
          </div>
          <a :href="'https://www.' + el.link">
            <div class="element_btn">more</div>
          </a>
        </div>
        <div class="list_element-lightning"></div>
      </div>
    </div>
  </div>
</template>

<script setup>
import logo_megapari_bw from './icons/logo_megapari_bw.svg';
import logo_megaslot_bw from './icons/logo_megaslot_bw.svg';
import logo_megaslot_bw_2 from './icons/logo_megaslot_bw_2.svg';
import logo_unislot_bw from './icons/logo_unislot_bw.svg';
import logo_megapari_color from './icons/logo_megapari_color.svg';
import logo_megaslot_color from './icons/logo_megaslot_color.svg';
import logo_megaslot_color_2 from './icons/logo_megaslot_color_2.svg';
import logo_unislot_color from './icons/logo_unislot_color.svg';

const partnerList = [
  {
    logo: logo_megapari_color,
    logo_dark: logo_megapari_bw,
    head: 'Megapari.com – Sportsbook online casino',
    link: 'megapari.com',
    body: 'Megapari offers sports betting, virtual sports, online casinos, and more than 10,000 games including slots, table games, and live dealer games.',
  },
  {
    logo: logo_unislot_color,
    logo_dark: logo_unislot_bw,
    head: 'Unislots.com Worldwide Online Casino',
    link: 'unislots.com',
    body: 'Unislots is an online casino that offers a wide range of slots, table games, and live dealer games.',
  },
  {
    logo: logo_megaslot_color,
    logo_dark: logo_megaslot_bw,
    head: 'Megaslot.io Online Casino',
    link: 'megaslot.io',
    body: 'Megaslot is an online casino that offers a wide range of slots, table games, and live dealer games.',
  },
  {
    logo: logo_megaslot_color_2,
    logo_dark: logo_megaslot_bw_2,
    head: 'Megaslot.com Online Casino',
    link: 'megaslot.com',
    body: 'Megaslot is an online casino that offers a wide range of slots, table games, and live dealer games.',
  },
];
</script>

<style scoped>
.partners_container {
  min-height: 822px;
  /* padding: 50px 100px; */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2em;
}
.partners_header {
  align-self: flex-start;
  width: 100%;
  padding: 22px 32px;
  background: #ffffff;
  border: 1px solid #282841;
  font-family: 'Oranienbaum';
  font-style: normal;
  font-weight: 400;
  font-size: 64px;
  line-height: 74px;
  text-transform: uppercase;
  color: #282841;
}
.partners_list {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 10px;
}
.list_element-container {
  position: relative;
  z-index: 0;
}
.list_element {
  position: inherit;
  z-index: 5;
  padding: 115px 70px;
  padding-bottom: 20px;
  height: 522px;
  width: 320px;
  background-color: #ffffff;
  border: 1px solid #282841;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  transition: 0.3s all ease-in-out;
  cursor: default;
}
.list_element-lightning {
  opacity: 0%;
  position: absolute;
  width: 8px;
  height: 8px;
  background: linear-gradient(91.52deg, #5df2fb -25.57%, #4790fe 85.06%);
  filter: blur(200px);
  transition: 0.5s all ease-in-out;
}
.list_element:hover {
  background-color: #040308;
  transform: rotate(8.73deg);
}
.list_element:hover > .element_logo {
  background-image: var(--hover_img_partners);
}
.list_element:hover .element_btn {
  display: flex;
}
.list_element-container:hover > .list_element-lightning {
  top: 0%;
  width: 408px;
  height: 408px;
  opacity: 100%;
}
.list_element:hover > .element_head,
.list_element:hover > .element_body {
  color: #ffffff;
}

.element_logo {
  height: 35px;
  width: 180px;
  margin-bottom: 25px;
  background-image: var(--img_partners);
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
}
.element_head {
  font-weight: 500;
  font-size: 16px;
  line-height: 18px;
  color: #282841;
  margin-bottom: 10px;
}
.element_link {
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  color: #4790fe;
  margin-bottom: 10px;
}
.element_body {
  font-weight: 300;
  font-size: 15px;
  line-height: 21px;
  color: #282841;
  margin-bottom: 9px;
}
.element_btn {
  display: none;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 90px;
  height: 40px;
  background-color: #4790fe;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  color: #ffffff;
}
.element_btn:hover {
  background-color: #ffffff;
  color: #4790fe;
}
</style>

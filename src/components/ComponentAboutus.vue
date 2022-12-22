<template>
  <div class="aboutus_container">
    <div class="aboutus_title">about&nbsp;us</div>
    <div class="aboutus_greeting">
      Hello! We are an affiliate program for online Gambling and online sports
      Betting
      <div class="logo_7token"></div>
      <div class="logo_1"></div>
      <div class="logo_777"></div>
    </div>
    <div class="aboutus_description">
      All brands included in MEGAPARTNERS have legal permission to conduct
      online gambling based on Curacao and MGA licenses. We guarantee
      reliability and stability both in providing services to our Players and in
      working with our Partners.
      <div class="logo_MPtoken"></div>
      <a href="">
        <div class="description_btn">read&nbsp;more</div>
      </a>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.aboutus_container {
  width: 100%;
  min-height: 800px;
  background-color: #282841;
  padding: 140px 100px;
  display: grid;
  grid-template-columns: 208px 2fr 2fr;
  gap: 2rem;
  min-width: 1172px;
}
.aboutus_title {
  font-family: 'Oranienbaum';
  font-style: normal;
  font-weight: 400;
  font-size: 160px;
  line-height: 208px;
  color: #f1f0f1;
  transform: rotate(-90deg) translateY(30%) translateX(-100%);
  z-index: 3;
}
.aboutus_title:first-letter {
  text-transform: uppercase;
}
.aboutus_greeting {
  position: relative;
  font-style: normal;
  font-weight: 300;
  font-size: 33px;
  line-height: 45px;
  color: #4790fe;
  max-width: 520px;
  min-width: 350px;
}
.aboutus_description {
  position: relative;
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  color: #f1f0f1;
  max-width: 550px;
  min-width: 350px;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: space-between;
}
.logo_7token {
  position: absolute;
  height: 106px;
  width: 106px;
  background-image: url('./icons/logo_7token.svg');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  top: 20%;
  left: -60%;
}
.logo_1 {
  position: absolute;
  width: 130px;
  height: 208px;
  background-image: url('./icons/logo_1.svg');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  top: 70%;
  left: -20%;
}
.logo_777 {
  position: absolute;
  width: 350px;
  height: 350px;
  background-image: url('./icons/logo_777.svg');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  top: 50%;
  right: -5%;
}
.logo_MPtoken {
  position: absolute;
  width: 295px;
  height: 225px;
  background-image: url('./icons/logo_MPtoken.png');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  top: 45%;
  left: 10%;
}
.description_btn {
  background-color: #4790fe;
  height: 50px;
  width: 160px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
  color: #282841;
  text-transform: uppercase;
  top: -20px;
}
.description_btn:hover {
  background-color: #ffffff;
}
</style>

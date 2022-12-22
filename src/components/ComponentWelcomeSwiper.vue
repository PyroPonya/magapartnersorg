<template>
  <swiper
    :pagination="{
      type: 'progressbar',
    }"
    :autoplay="{
      delay: 6000,
      disableOnInteraction: false,
    }"
    :loop="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide v-for="(el, id) in slideArr" :key="id" class="slide">
      <div class="">
        <img :src="el" alt="bad_error_why" />
        <a href="https://backoffice.megapartners.org/partner/register">
          <div class="section_btn">become&nbsp;a&nbsp;partner</div>
        </a>
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';
import 'swiper/css/navigation';

// import required modules
import { Autoplay, Pagination } from 'swiper';
import slide_1 from './icons/slider_welcome_desk.jpg';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const slideArr = [slide_1, slide_1, slide_1, slide_1, slide_1];
    return {
      modules: [Autoplay, Pagination],
      slideArr,
    };
  },
};
</script>
<style scoped>
.swiper,
.mySwiper {
  min-width: 100%;
  max-width: 100%;
  min-height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;
  background: none;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}

.swiper-slide img {
  /* change slide hight @here */
  display: block;
  width: 100%;
  height: 100%;
  object-fit: contain;
  position: relative;
}
.section_btn {
  position: absolute;
  bottom: 1rem;
  right: 1rem;
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
}
</style>

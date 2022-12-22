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
    <swiper-slide v-for="(el, id) in slideArr" :key="id" class="slide"
      ><img :src="el" alt="bad_error_why" />
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
}
</style>

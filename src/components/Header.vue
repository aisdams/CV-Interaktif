<template>
  <header>
    <nav class="navnya">
      <ul>
        <li><a href="">Aisyah Ramadhani</a></li>
        <li><a href="">About</a></li>
        <li><a href="">Project</a></li>
      </ul>
  </nav>
  </header>
  <swiper
    :effect="'cards'"
    :grabCursor="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide><img src="https://cdn.medcom.id/dynamic/content/2021/12/21/1367210/EfVzJA7KQF.jpg?w=480" alt=""></swiper-slide>
    <swiper-slide><img src="https://www.roberthalf.com/sites/default/files/styles/full_width_content_image_1x_small_480/public/2017-12/Data%20Analyst.jpg?itok=wl9XqQFD" alt=""></swiper-slide
    >
    <swiper-slide><img src="https://campuspedia.id/news/wp-content/uploads/2021/06/82.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="https://blue.kumparan.com/image/upload/fl_progressive,fl_lossy,c_fill,q_auto:best,f_jpg,w_480/kjvuulvftrvz6aimfi1k.jpg" alt=""></swiper-slide
    >
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-cards";

import "./style.css";

// import required modules
import { EffectCards } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCards],
    };
  },
};
</script>

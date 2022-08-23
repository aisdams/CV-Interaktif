<template>
  <div class="about d-flex">
    <div class="textnya">
    <h1 class="mb-5">About Me</h1>
    <p>Name : Aisyah Ramadhani</p>
    <p>Role : Software Developer</p>
    <p>Phone : +62 82258374851</p>
    <p>Email : aisyahrmdh14@gmail.com</p>
    <p>Alamat : Jl Tungkal 3 Depok, Indonesia | 16418</p>
    </div>

    <ul class="list-unstyled card-body mb-0 pb-0 progressnya">
    <li class="row mb-3">
      <p>HTML, CSS, JavaScript</p>
      <div class="col-7 align-self-center">
        <p style="position: absolute; top: -1.5rem; left: 27rem;">75%</p> 
        <div class="progress" style="height: 5px; width: 28rem;">
          <div class="progress-bar bg-primary" role="progressbar" style="width: 75%" aria-valuenow="15" aria-valuemin="0" aria-valuemax="100"></div>
        </div>
      </div>
    </li>
    <li class="row mb-3">
      <p>PHP & Mysql</p>
      <div class="col-7 align-self-center">
        <p style="position: absolute; top: -1.5rem; left: 27rem;">70%</p> 
        <div class="progress" style="height: 5px; width: 28rem;">
          <div class="progress-bar bg-primary" role="progressbar" style="width: 70%" aria-valuenow="15" aria-valuemin="0" aria-valuemax="100"></div>
        </div>
      </div>
    </li>
    <li class="row mb-3">
      <p>React & Laravel</p>
      <div class="col-7 align-self-center">
        <p style="position: absolute; top: -1.5rem; left: 27rem;">80%</p> 
        <div class="progress" style="height: 5px; width: 28rem;">
          <div class="progress-bar bg-primary" role="progressbar" style="width: 80%" aria-valuenow="15" aria-valuemin="0" aria-valuemax="100"></div>
        </div>
      </div>
    </li>
    <li class="row mb-3">
      <p>UI/UX Design</p>
      <div class="col-7 align-self-center">
        <p style="position: absolute; top: -1.5rem; left: 27rem;">90%</p> 
        <div class="progress" style="height: 5px; width: 28rem;">
          <div class="progress-bar bg-primary" role="progressbar" style="width: 90%" aria-valuenow="15" aria-valuemin="0" aria-valuemax="100"></div>
        </div>
      </div>
    </li>
  </ul>
  </div>

<div class="swipperjs">
  <swiper
    :slidesPerView="5"
    :centeredSlides="true"
    :spaceBetween="30"
    :autoplay="{
      delay: 1500,
      disableOnInteraction: false,
    }"
    :modules="modules"
    class="mySwiper">
    <swiper-slide><img src="@/assets/figma.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/adobe-xd.svg" alt=""></swiper-slide
    ><swiper-slide><img src="@/assets/html.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/css.svg" alt=""></swiper-slide
    ><swiper-slide><img src="@/assets/php.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/adobe-photoshop.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/react.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/laravel.svg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/wordpress.svg" alt=""></swiper-slide>
  </swiper>
</div>
  
</template>

<script>
import "../about.css";
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";


import { Autoplay, Pagination } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [ Autoplay],
    };
  },
};
</script>
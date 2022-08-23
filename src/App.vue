<template>
  <header>
    <transition
    appear
    @before-enter="beforeEnter"
    @enter="enter"
  >
    <nav class="navnya">
      <ul>
        <li class="logonya"><a href="">Aisyah<span style="color: blue;">Ramadhani</span></a></li>
        <li class="menu-center"><RouterLink to="/">Personal</RouterLink></li>
        <li class="menu-center"><RouterLink to="/skill">Skill</RouterLink></li>
        <li class="menu-center"><a href="@/assets/Cv magang Aisyah Ramadhani new.pdf" download>CV</a></li>
        <li><button><RouterLink to="/contactus" style="text-decoration: none; color: #fff;">Contact us</RouterLink></button></li>
      </ul>
  </nav>
  </transition>
  <div class="square">
    <div class="circlenya"></div>
    <img alt="Love logo" class="logo" src="@/assets/love.svg" width="15" height="15" />
    <h4>Software Developer</h4>
    <h1>Hi I'm Aisyah Ramadhani</h1>
    <p>Saya adalah siswi magang dari SMK Taruna Bhakti tetapi saya yakin bahwa saya memenuhi syarat untuk posisi itu karena keterampilan saya sesuai dengan persyaratan. Sekolah IT jurusan pemrograman komputer dengan latar belakang Java, HTML, CSS, MySQL, Laravel, MongoDB, React, dan Desain UI&UX</p>
    <button class="btn-hire"><a href="" style="text-decoration: none; color: #fff;font-size: 15px;">Hire Me</a></button>
    <div class="sosialmedia">
      <a href="https://www.instagram.com/aisrdm_14/" target=”_blank”><img src="@/assets/instagram.svg" alt="" width="45" height="45" /></a>
      <a href="https://github.com/aisdams/" target=”_blank”><img src="@/assets/github.svg" alt="" width="45" height="45" /></a>
      <a href="https://www.linkedin.com/in/aisyah-ramadhani-6b010420b/" target=”_blank”><img src="@/assets/linkedin.svg" alt="" width="45" height="45" /></a>
      <a href="#"><img src="@/assets/facebook.svg" alt="" width="45" height="45" /></a>
    </div>
  </div>

  </header>
  <div class="banner circle">
    <img src="@/assets/self.png" alt="" style="position: relative; left: -3.5rem">
  </div>

  <RouterView />
  
</template>

<script>
import { RouterLink, RouterView } from 'vue-router'
// Import Swiper Vue.js components
import gsap from 'gsap'

// Import styles

import "./style.css";

export default {
  methods: {
    // where the animation will start from
    beforeEnter(el) {
      el.style.opacity = '0'
      el.style.transform = 'translateY(-100px)'
    },
    // where the animation will end up
    enter(el) {
      gsap.to(el, {
        duration: 1,
        y: 0,
        opacity: 1,
      })
    }
  },
  data() {
    return {
      
    }
  },
  mounted: function(){
    gsap.fromTo('.circle',{opacity:0 }, {opacity: 1 , x: 20 , duration: 1, delay: 2 });
    gsap.fromTo('.square', {opacity:0, x: 20}, { opacity:1, x: 20 , duration: 1, delay: 2 });
  },
};
</script>

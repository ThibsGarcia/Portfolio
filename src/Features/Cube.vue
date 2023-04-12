<script lang="ts">
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from "swiper/vue";
  
  // Import Swiper styles
  import "swiper/css";
  
  import "swiper/css/effect-cube";
  import "swiper/css/pagination";
  
  
  // import required modules
  import { EffectCube, Pagination, Mousewheel, Keyboard } from "swiper";
  
  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [EffectCube, Pagination, Mousewheel, Keyboard],
      };
    },
  };
  </script>

<template>
      <div class="big-slide">

        <div v-motion
                    :initial="{ opacity: 0, x: 200 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="800" 
        class="slide-container">
            <swiper
            :effect="'cube'"
            :grabCursor="true"
            :mousewheel="true"
            :keyboard="{
            enabled: true,
            }"
            :rewind="true"
            :cubeEffect="{
                shadow: true,
                slideShadows: true,
                shadowOffset: 20,
                shadowScale: 0.94,
            }"
            :pagination="{
                clickable: true,
            }"
            :modules="modules"
            class="mySwiper"
            >
            <swiper-slide>
                <img src="../assets/img/html.png"/>
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/img/css.png" />
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/img/js.png" />
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/img/Tailwind.png"/>
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/img/vue.png" />
                
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/img/typescript.png" />
            </swiper-slide>
            </swiper>
        </div>
    </div>
  </template>
  
  <style lang="scss" scoped>
@media screen and (max-width: 640px) {
  .big-slide {
  display: flex;
  justify-content: center;
  height: 100%;
  }
  .slide-container {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 80%;
    height: 80%;
  }
  .swiper {
    width: 200px;
    height: 200px;
  }
  .swiper-slide {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-size: cover;
      width: 200px;
      height: 200px;
      background-size: cover;
      border-radius: 10%;
  }
  .swiper-slide img {
    display: block;
    width: 45%;
    height: 45%;
  }
  .slide-container {
    transition: all 0.7s ease-out;
  }
}
@media screen and (min-width: 640px) {
  .big-slide {
  display: flex;
  justify-content: center;
  height: 100%;
  }

  .slide-container {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 80%;
    height: 80%;
  }


  .swiper {
    width: 200px;
    height: 200px;
  }

  .swiper-slide {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-size: cover;
      width: 200px;
      height: 200px;
      background-size: cover;
      border-radius: 10%;
  }

  .swiper-slide img {
    display: block;
    width: 45%;
    height: 45%;
  }
  .slide-container {
    transition: all 0.7s ease-out;
  }
}
@media screen and (min-width: 768px) {
}


</style>
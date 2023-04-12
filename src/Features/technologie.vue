<script lang="ts">
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-coverflow";
import "swiper/css/pagination";


// import required modules
import { EffectCoverflow, Pagination, Mousewheel, Keyboard } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCoverflow, Pagination, Mousewheel, Keyboard],
    };
  },
};
</script>

<template>
      <div class="big-slide flex flex-col">
        <div class="slide-title text-center">
          <h2 class="text-5xl font-semibold">Langages Utilisés</h2>
        </div>

        <div class="slide-container">
            <swiper
            :effect="'coverflow'"
            :slidesPerView="'auto'"
            :mousewheel="true"
            :grabCursor="true"
            :centeredSlides="true"
            :rewind="true"
            :keyboard="{
            enabled: true,
            }"
            :coverflowEffect="{
                rotate: 50,
                stretch: 0,
                depth: 100,
                modifier: 1,
                slideShadows: true,
            }"
            :pagination="{
              clickable: true,
            }"
            :modules="modules"
            class="mySwiper"
            >
                <swiper-slide >
                    <img src="../assets/img/html.png"/>
                </swiper-slide>
                <swiper-slide >
                    <img src="../assets/img/css.png"/>
                </swiper-slide>
                <swiper-slide >
                    <img src="../assets/img/js.png"/>
                </swiper-slide>
                <swiper-slide >
                    <div class="test-back">
                        <img src="../assets/img/vue.png"/>
                    </div>
                </swiper-slide>
                <swiper-slide >
                    <div class="test-back">
                        <img src="../assets/img/Tailwind.png"/>
                    </div>
                </swiper-slide>
                <swiper-slide >
                    <img src="../assets/img/typescript.png"/>
                </swiper-slide>
            </swiper>
        </div>
    </div>
  </template>
 
  <style scoped lang="scss"> 
.big-slide {
  display: flex;
  justify-content: center;
   height: 50vh;
}
.slide-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
  width: 90%;
}

.swiper {
  width: 100%;
  padding-bottom: 50px;
}

.swiper-slide {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-size: cover;
     width: 230px;
     height: 230px;
    background-size: cover;
    background-image: url(../assets/img/back-slide.jpg);
    border-radius: 10%;
    &:hover {
      transform: scale(1.2);
    }
}
.test-back {
    width: 30%;
    height: 19%;
    background-color: #370e68;
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;

    img {
        position: absolute;
    }
}
.swiper-slide img {
  display: block;
  width: 35%;
  height: 35%;
  border-radius: 20%;
}

  </style>
  
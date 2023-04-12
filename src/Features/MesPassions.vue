<script lang="ts">
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/effect-cards';
  import 'swiper/css/navigation';


  // import required modules
  import { EffectCards, Mousewheel, Keyboard, Navigation } from 'swiper';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [EffectCards, Mousewheel, Keyboard, Navigation],
      };
    },
  };
</script>
<template>
  <div class="big-slide">
    <div class="slide-container flex flex-col">
      <div v-motion-slide-visible-top class="title flex items-center">
        <h2 class="text-xl sm:text-4xl">Mes centres d'intérêts</h2>
      </div>
      <swiper
        :effect="'cards'"
        :grabCursor="true"
        :mousewheel="true"
        :rewind="true"
        :modules="modules"
        class="mySwiper"
        :keyboard="{
          enabled: true,
        }"
         :navigation="{
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        }"
        v-motion-slide-visible-right>
        <swiper-slide>
          <div class="slide-content">
          <h2>Voyage</h2>
          </div>
        </swiper-slide>
    
        <swiper-slide>
          <div class="slide-content">
          <h2>Musique</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Sport</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Activités Plein Air</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Photographie</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Construction en Génie Civil</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Technologies Innovantes</h2>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="slide-content">
          <h2>Exploration Spatiale</h2>
          </div>
        </swiper-slide>
       
       
        
        <div class="swiper-pagination" slot="pagination"></div>
       
      </swiper>
    
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>
    </div>

    
  </div>
    
</template>

<style lang="scss" scoped>
@media screen and (max-width: 640px) {
  .big-slide {
  display: flex;
  justify-content: center;
  width: 75%;
}
.title {
  height: 20%;
}
.slide-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60vh;
  width: 100%;
}

.swiper {
  width: 90%;
  height: 65%;
}

.swiper-slide {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 18px;
  font-size: 26px;
  font-weight: bold;
  color: #fff;
}

.swiper-slide:nth-child(1n) {
  background-image: url(../assets/img/voyage.jpg);
  background-size: cover;
}

.swiper-slide:nth-child(2n) {
    background-image: url(../assets/img/musique.jpg);
    background-size: cover;
}

.swiper-slide:nth-child(3n) {
    background-image: url(../assets/img/sport.jpg);
    background-size: cover;
}

.swiper-slide:nth-child(4n) {
    background-image: url(../assets/img/activté-2.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(5n) {
    background-image: url(../assets/img/photographie.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(6n) {
    background-image: url(../assets/img/Milau.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(7n) {
    background-image: url(../assets/img/technologie.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(8n) {
    background-image: url(../assets/img/space.jpg);
    background-size: cover;
}
.swiper-button-next,
.swiper-button-prev {
  position: absolute;
  top: 60%;
  width: 60px;
  height: 60px;
  cursor: pointer;
}
.swiper-button-next:after,.swiper-button-prev:after {
    color: red;
}
.swiper-button-next {
  right: -20%;
}
.swiper-button-prev{
  left: -20%;
}

.slide-content {
    position: absolute;
    top: 85%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    width: 80%;
  }
}
@media screen and (min-width: 640px) {
  .big-slide {
  display: flex;
  justify-content: center;
  width: 75%;
}
.title {
  height: 20%;
}
.slide-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60vh;
  width: 100%;
}

.swiper {
  width: 90%;
  height: 75%;
}

.swiper-slide {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 18px;
  font-size: 26px;
  font-weight: bold;
  color: #fff;
}

.swiper-slide:nth-child(1n) {
  background-image: url(../assets/img/voyage.jpg);
  background-size: cover;
}

.swiper-slide:nth-child(2n) {
    background-image: url(../assets/img/musique.jpg);
    background-size: cover;
}

.swiper-slide:nth-child(3n) {
    background-image: url(../assets/img/sport.jpg);
    background-size: cover;
}

.swiper-slide:nth-child(4n) {
    background-image: url(../assets/img/activté-2.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(5n) {
    background-image: url(../assets/img/photographie.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(6n) {
    background-image: url(../assets/img/Milau.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(7n) {
    background-image: url(../assets/img/technologie.jpg);
    background-size: cover;
}
.swiper-slide:nth-child(8n) {
    background-image: url(../assets/img/space.jpg);
    background-size: cover;
}
.swiper-button-next,
.swiper-button-prev {
  position: absolute;
  top: 60%;
  width: 60px;
  height: 60px;
  cursor: pointer;
}
.swiper-button-next:after,.swiper-button-prev:after {
    color: red;
}
.swiper-button-next {
  right: -20%;
}
.swiper-button-prev{
  left: -20%;
}

.slide-content {
    position: absolute;
    top: 85%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    width: 80%;
  }
}
@media screen and (min-width: 768px) {
}
@media screen and (min-width: 1024px) {
  .big-slide {
  width: 65%;
}
}
@media screen and (min-width: 1280px) {
  .big-slide {
  width: 45%;
}
}


</style>

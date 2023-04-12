<script setup lang="ts">
import technologie from '@/Features/technologie.vue'
</script>

<template>
    <div class="what">
        <div class="content-what flex flex-col justify-around">
           <div class="top-content-what flex flex-col justify-around">
                <h6 v-motion-slide-visible-bottom
                class="text-3xl md:text-4xl animation-05">Mes Objectifs</h6>
                <h3 v-motion-slide-visible-bottom 
                class="text-xl md:text-2xl animation-05">Je nourris ma passion en apprenant constamment pour devenir un développeur plus compétent.<br> Tout en cultivant ma créativité et mon efficacité pour offrir des solutions innovantes.<br></h3>
            </div> 
            <div class="ligne"></div>
            <div class="title-content-what flex flex-col justify-around">
                <h2 v-motion-slide-visible-bottom
                class="text-6xl md:text-7xl lg:text-8xl xl:text-9xl font-semibold animation-05">Penser. Créer. Ajuster.</h2>
            </div>
        </div>
        <div class="block-3d">
            <img v-motion-slide-visible-left class="white-block animation-07" src="../assets/img/figure-2.png" alt="white-block">
            <img v-motion-slide-visible-right class="white-blur-block animation-07" src="../assets/img/figure-1.png" alt="white-blur-block">
            <img v-motion-slide-visible-bottom class="pink-block animation-07" src="../assets/img/main-pic-1.png" alt="pink-block">
        </div>
    </div>
    <technologie v-motion-slide-visible-bottom class="animation-05"/>

</template>

<style scoped lang="scss">
    @media screen and (max-width: 640px) {
        .what {
        width: 90%;
        height: 80vh;
        margin: auto;
        .content-what {
            height: 100%;
            width: 100%;
            padding-bottom: 80px;
        }
        .top-content-what {
            width: 100%;
            height: 40%;
        }
        .ligne {
            height: 1px;
            background-color: #e3a1bf;
            width: 40%;
        }
        .title-content-what {
            height: 50%;
        }
        .button {
            display: inline-flex;
        }
        .btn-1 {
            width: 100%;
            height: 80px;
            background-color: #4C40F7;
            border-radius: 20px;
            color: white;
            cursor: pointer;
        }
       .block-3d {
        position: absolute;
        .white-block {
         display: none;
        }
        .white-blur-block {
         display: none;
        }
        .pink-block{
         position: relative;
         top: -550px;
         left: 40%;
         width: 50px;
         overflow: hidden;
        }
       }
}
}
@media screen and (min-width: 640px) {
    .what {
        width: 90%;
        height: 80vh;
        margin: auto;
        .content-what {
            height: 100%;
            width: 80%;
        }
        .top-content-what {
            width: 100%;
            height: 40%;
        }
        .ligne {
            height: 1px;
            background-color: #e3a1bf;
            width: 40%;
        }
        .title-content-what {
            height: 50%;
        }
        .button {
            display: inline-flex;
        }
        .btn-1 {
            width: 266px;
            height: 80px;
            background-color: #4C40F7;
            border-radius: 20px;
            color: white;
            cursor: pointer;
        }
       .block-3d {
        position: absolute;
        .white-block {
         position: relative;
         top: -200px;
         right: -300px;
         width: 250px;
        }
        .white-blur-block {
         position: relative;
         width: 180px;
         top: -500px;
         right: -430px;
        }
        .pink-block{
         position: relative;
         top: -1050px;
         left: 140%;
         width: 170px;
        }
       }
}
}

@media screen and (min-width: 768px) {
    .what {
        width: 90%;
        height: 80vh;
        margin: auto;
        .content-what {
            height: 100%;
            width: 80%;
        }
        .top-content-what {
            width: 100%;
            height: 40%;
        }
        .ligne {
            height: 1px;
            background-color: #e3a1bf;
            width: 40%;
        }
        .title-content-what {
            height: 50%;
        }
        .button {
            display: inline-flex;
        }
        .btn-1 {
            width: 266px;
            height: 80px;
            background-color: #4C40F7;
            border-radius: 20px;
            color: white;
            cursor: pointer;
        }
       .block-3d {
        position: absolute;
        .white-block {
         position: relative;
         top: -200px;
         right: -300px;
         width: 250px;
        }
        .white-blur-block {
         position: relative;
         width: 180px;
         top: -500px;
         right: -430px;
        }
        .pink-block{
         position: relative;
         top: -880px;
         left: 160%;
         width: 100px;
        }
       }
}

}

@media screen and (min-width: 1024px) {
    .what {
        width: 80%;
        height: 100vh;
        margin: auto;
        .content-what {
            height: 100%;
            width: 80%;
            margin: auto;
        }
        .top-content-what {
            width: 75%;
            height: 40%;
        }
        .ligne {
            height: 1px;
            background-color: #e3a1bf;
            width: 40%;
        }
        .title-content-what {
            height: 50%;
        }
        .button {
            display: inline-flex;
        }
        .btn-1 {
            width: 266px;
            height: 80px;
            background-color: #4C40F7;
            border-radius: 20px;
            color: white;
            cursor: pointer;
        }
       .block-3d {
        position: absolute;
        .white-block {
         position: relative;
         top: -200px;
         right: -530px;
         width: 250px;
        }
        .white-blur-block {
         position: relative;
         width: 180px;
         top: -580px;
         right: -650px;
        }
        .pink-block{
         position: relative;
         top: -1050px;
         left: 270%;
         width: 200px;
        }
       }
}
@media screen and (min-width: 1280px) {
        .what{
            .block-3d{
                .pink-block{
                    top: -1100px;
                    left: 420%;
                }
            }
        }
    }

}
</style>

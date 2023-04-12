<script setup lang="ts">
import type { Page } from '@/Interfaces/type';
import { reactive } from 'vue';

const state = reactive({
    open: false
})
const props = defineProps<{
    page: Page
}>()
const emit = defineEmits<{
    (e: 'navigate', page : Page) : void ;
}>()
</script>

<template>
  <div class="header pt-10">
                <nav class="header-config flex justify-between items-center">
                    <div class="header-left flex justify-between items-center">
                        <div   v-motion
                                :initial="{ opacity: 0, x: -50 }"
                                :enter="{ opacity: 1, x: 0, scale: 1 }"
                                :hovered="{ scale: 1.02 }"
                                :delay="300"
                        @click="emit('navigate', 'HomePage')" class="logo flex justify-between items-center animation-05">
                            <img class="logo-picture" src="../assets/img/LOGO-LAXAA.png" alt="logo-thibs">
                            <h3 class="lg:text-lg xl:text-xl font-semibold" >Thibault Garcia</h3>
                        </div>
                        <div v-motion
                                :initial="{ opacity: 0, y: -100 }"
                                :enter="{ opacity: 1, y: 0, scale: 1 }"
                                :hovered="{ scale: 1.02 }"
                                :delay="600"
                        class="menu-header flex justify-around animation-05">
                            <h5 class="lg:text-lg xl:text-xl font-semibold" @click="emit('navigate', 'AboutMe')">À propos de moi</h5>
                            <h5 class="lg:text-lg xl:text-xl font-semibold" @click="emit('navigate', 'BoutiqueProject')">Projet</h5>
                        </div>
                    </div>
                    <div class="header-right flex items-center">
                        <div v-motion
                                :initial="{ opacity: 0, x: 50 }"
                                :enter="{ opacity: 1, x: 0, scale: 1 }"
                                :hovered="{ scale: 1.02 }"
                                :delay="900"
                        @click="state.open = true" class="menu-logo flex flex-col justify-around animation-05">
                            <div class="ligne-top"></div>
                            <div class="ligne-bottom"></div>
                        </div>
                    </div>
                </nav>
                <div v-if="state.open">
                    <div class="big-menu flex">
                        <div class="big-menu-left flex items-center">
                            <div v-motion
                                :initial="{ opacity: 0, x: -80 }"
                                :enter="{ opacity: 1, x: 0, scale: 1 }"
                                :hovered="{ scale: 1.02 }"
                                :delay="200" class="object-menu-left animation-05"></div>
                        </div>
                        <div class="big-menu-right">
                            <div class="big-menu-right-content flex flex-col justify-around">
                                    <div class="top-right flex justify-end">
                                        <div class="top-right-logo">
                                            <div  v-motion
                                                :initial="{ opacity: 0, x: 70 }"
                                                :enter="{ opacity: 1, x: 0, scale: 1 }"
                                                :hovered="{ scale: 1.02 }"
                                                :delay="200" 
                                            @click="state.open = false" class="top-right-logo-content flex items-center justify-center animation-05">
                                                <div class="ligne-top-menu"></div>
                                                <div class="ligne-bottom-menu"></div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="center-right flex justify-between">
                                        <div class="center-left flex flex-col justify-between">
                                                <div v-motion
                                                    :initial="{ opacity: 0, y: -50 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="200"  
                                                class="text flex items-center animation-03">
                                                    <img class="mr-10 w-8" src="../assets/icons/email.svg" alt="icon">
                                                    <h5 class="text-base xl:text-2xl">thibaultgarcia.64@gmail.com</h5>
                                                </div>
                                                <div v-motion
                                                    :initial="{ opacity: 0, y: -50 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="400" 
                                                class="text flex items-center animation-03">
                                                    <img class="mr-10 w-8" src="../assets/icons/place.svg" alt="icon">
                                                    <h5 class="text-base xl:text-2xl">Ascain, Pays Basque, France</h5>
                                                </div>
                                                <div v-motion
                                                    :initial="{ opacity: 0, y: -50 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="600" 
                                                class="text flex items-center animation-03">
                                                    <img class="mr-10 w-8" src="../assets/icons/phone.svg" alt="icon">
                                                    <h5 class="text-base xl:text-2xl"> 06 65 55 83 47</h5>
                                                </div>
                                        </div>
                                        <div class="center-right flex flex-col justify-between">
                                            <h2  v-motion
                                                    :initial="{ opacity: 0, y:50 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="100" 
                                                    @click="emit('navigate', 'AboutMe')"
                                            class="text-2xl lg:text-4xl xl:text-6xl font-semibold title-big-menu animation-05">À propos de moi</h2>
                                            <h2 v-motion
                                                    :initial="{ opacity: 0, y:50 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="300"
                                                    @click="emit('navigate', 'BoutiqueProject')"
                                            class="text-2xl lg:text-4xl xl:text-6xl font-semibold title-big-menu animation-05">Projet</h2>
                                            <h2 v-motion
                                                    :initial="{ opacity: 0, y:50}"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="500"
                                                    @click="emit('navigate', 'HomePage')"
                                            class="text-2xl lg:text-4xl xl:text-6xl font-semibold title-big-menu animation-05">Accueil</h2>
                                            
                                        </div>
                                    </div>
                                    <div class="down-right flex justify-between">
                                        <div v-motion
                                                    :initial="{ opacity: 0, y: 300 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="100"  
                                                    class="icone-down flex justify-between items-center animation-05">
                                            <img class="logo-down" src="../assets/icons/linkedin.png" alt="linkedin">
                                            <a href="https://www.linkedin.com/in/thibault-garcia-461b35161/" target="_blank" rel="noopener noreferrer"><h4 class="text-base">Linkedin</h4></a>

                                        </div>
                                        <div v-motion
                                                    :initial="{ opacity: 0, y: 300 }"
                                                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                                                    :hovered="{ scale: 1.02 }"
                                                    :delay="300" 
                                                    :duration="1000"
                                        class="icone-down flex justify-between items-center animation-05">
                                            <img class="logo-down" src="../assets/icons/linkedin.png" alt="linkedin">
                                            <a href="https://www.linkedin.com/in/thibault-garcia-461b35161/" target="_blank" rel="noopener noreferrer"><h4 class="text-base">Linkedin</h4></a>
                                        </div>
                                    </div>
                            </div>
                        </div>
                        <div class="back-mobile">
                            <img src="../assets/img/bg-header-mobile.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
</template>

<style scoped lang="scss">
    @media screen and (max-width: 640px) {
        .header{
            padding: 0;
        }
        .header-config {
        height: 80px;
        width: 90%;
        margin: auto;
    } 
    .header-left {
        width: 70%;
        height: 100%;
    }
    .center-right{
        z-index: 1;
    }
    .logo-picture {
        width: 40%;
    }
    .top-right{
        width: 90%;
    }
    .logo {
        width: 45%;
        height: 45px;
        h3{
            display: none;
        }
    }
    .menu-header {
        width: 45%;
        display: none;
    }
    .header {
        width: 100%;
    }
    .header-right {
        height: 100%;
        .menu-logo {
            height: 60%;
            cursor: pointer;
        }
    }
    /**Big menu */
    .big-menu {
        position: fixed;
        top: 0px;
        left: 0px;
        width: 100vw;
        height: 100vh;
        background-color: #ffffff;
        display: flex;
        flex-direction: column;
        .big-menu-left {
            display: none;
        }
       
        .big-menu-right {
            height: 70vh;
            width: 100%;
        }
        .big-menu-right-content {
            position: relative;
            height: 90%;
            width: 80%;
            margin: auto;
        }
        .top-right-logo{
            z-index: 1;
        }
        .top-right-logo-content {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #4c40f7;
            position: relative;
            top: 50%;
            transition: 0.2s;
            &:hover {
                transform: scale(1.1);
            }
        }
        .ligne-top-menu {
        height: 3px;
        background-color: #ffffff;
        width: 30px;
        transform: rotate(45deg);
        position: absolute;
        }
        .ligne-bottom-menu{
        height: 3px;
        background-color: #ffffff;
        width: 30px;
        transform: rotate(-45deg);
        position: absolute;
        }
        .center-right {
            height: 230px;
            z-index: 2;
        }
        .center-left {
            display: none;
        }
        .down-right {
            width: 60%;
        }
        .down-right > :nth-child(1){
            display: none;
        }
        .icone-down {
            width: 70%;
            height: 80px;
            border-radius: 24px;
            transition: 0.2s;
        }
        .logo-down {
            height: 60%;
            }
        .icone-down:hover {
            box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
            transform: scale(1.1);
        }
        .title-big-menu:hover {
            color: #4c40f7;
        }
    
    }
    .ligne-top, .ligne-bottom {
        height: 1px;
        background-color: gray;
        width: 32px;
    }
    .back-mobile{
        position: absolute;
        height: 100vh;
        z-index: 0;
        img {
            position: relative;
            top: 0px;
            right: 0px;
            height: 100vh;
            width: 100vw;
        }
    }

}
@media screen and (min-width: 640px) {
    .header-config {
        height: 60px;
        width: 90%;
        margin: auto;
    } 
    .header-left {
        width: 70%;
    }
    .logo-picture {
        width: 20%;
    }
    .logo {
        width: 45%;
    }
    .menu-header {
        width: 45%;
    }
    .header {
        width: 100%;
    }
    .header-right {
        height: 100%;
        .menu-logo {
            height: 60%;
            cursor: pointer;
        }
    }
    /**Big menu */
    .big-menu {
        position: fixed;
        top: 0px;
        left: 0px;
        width: 100%;
        height: 100vh;
        background-color: #ffffff;
        .big-menu-left {
            width: 26%;
            height: 100vh;
            background-color: #1c1c87;
        }
        .object-menu-left {
            background-image: url(../assets/img/bg-header.png);
            height: 100%;
            width: 100%;
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
        }
        .big-menu-right {
            height: 100vh;
            width: 72%;
        }
        .big-menu-right-content {
            height: 100%;
            width: 78%;
            margin: auto;
        }
        .top-right-logo-content {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            background-color: #4c40f7;
            position: relative;
            transition: 0.2s;
            &:hover {
                transform: scale(1.1);
            }
        }
        .ligne-top-menu {
        height: 3px;
        background-color: #ffffff;
        width: 50px;
        transform: rotate(45deg);
        position: absolute;
        }
        .ligne-bottom-menu{
        height: 3px;
        background-color: #ffffff;
        width: 50px;
        transform: rotate(-45deg);
        position: absolute;
        }
        .center-right {
            height: 280px;
            cursor: pointer;
            z-index: 2;
        }
        .center-left {
            height: 192px;
            cursor: pointer;
        }
        .down-right {
            width: 90%;
        }
        .icone-down {
            width: 30%;
            height: 80px;
            border-radius: 24px;
            transition: 0.2s;
        }
        .logo-down {
            height: 60%;
            }
        .icone-down:hover {
            box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
            transform: scale(1.1);
        }
        .title-big-menu:hover {
            color: #4c40f7;
        }
    
    }
    .ligne-top, .ligne-bottom {
        height: 1px;
        background-color: gray;
        width: 32px;
    }
    .back-mobile{
        display: none;
    }
}

@media screen and (min-width: 768px) {
    .header-config{
        .header-left {
            width: 60%;
        }
    }
}
@media screen and (min-width: 1024px) {
        .big-menu{
            .object-menu-left {
            background-position: left;
            }
            .down-right{
                width: 70%;
            }
        }
    }

    @media screen and (min-width: 1280px) {
    .header{
        .big-menu{
            .down-right{
                width: 50%;
            }
        }
    }
}
</style>

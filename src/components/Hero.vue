<script setup lang="ts">
import { reactive } from 'vue';

const state = reactive({
    open: false
})
</script>

<template>
    <div class="hero">
        <div class="hero-text ">
            <h2 v-motion
                    :initial="{ opacity: 0, x: -200 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="300"
             class="font-bold text-4xl md:text-5xl xl:text-6xl">Hey, je m'appelle Thibault.</h2>

                <h2 v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="600"
                class="font-bold text-4xl md:text-5xl xl:text-6xl">Je suis Développeur Front-end.</h2> 
        </div>

        <div class="object-3d">
            <img  v-motion
                    :initial="{ opacity: 0, y: 100 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="1200" 
             class="purple-base animation-07" src="../assets/img/main-pic-6.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, x: 150 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="1000" 
             class="yellow-rectangle animation-07" src="../assets/img/main-pic-4.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, x: -500 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="800" 
             class="blue-block animation-07" src="../assets/img/main-pic-3.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, x: 150 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="600" 
                    
            class="purple-light-block animation-07" src="../assets/img/main-pic-2.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, y: -400 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="400" 
             class="pink-block animation-07" src="../assets/img/main-pic-1.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, y: -500 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.05 }"
                    :delay="500"
                class="orange-ball animation-07" src="../assets/img/main-pic-5.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, y: 300 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.05 }"
                    :delay="400"
            class="small-pink-block animation-07" src="../assets/img/figure-3.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, y: -300 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.05 }"
                    :delay="400"
            class="white-block animation-07" src="../assets/img/figure-2.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, x: -300 }"
                    :enter="{ opacity: 1, x: 0, scale: 1 }"
                    :hovered="{ scale: 1.05 }"
                    :delay="400"
            class="blur-white-block animation-07" src="../assets/img/figure-1.png" alt="object-3d">

            <img v-motion
                    :initial="{ opacity: 0, y: -500 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.05 }"
                    :delay="600"
            class="white-ball animation-07" src="../assets/img/main-pic-7.png" alt="object-3d">
        </div>
        <div v-motion
                    :initial="{ opacity: 0, y: -500 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="1000"
        class="scroll-down flex items-center space-between">
            <div class="scroll-button flex justify-center items-center shadow-2xl mr-5">
                <img class="scroll-button-img" src="../assets/img/scroll.svg" alt="scroll-button">
            </div>
            <h6>Scroll</h6>
        </div>
    </div>
    
    </template>
    
    <style scoped lang="scss">
@media screen and (max-width: 640px) {
    .hero {
        background-image: url(../assets/img/bg-main.jpg);
        height: 110vh;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .hero-text {
            position: absolute;
            top: 15%;
            left: 10%;
            width: 65%;
            height: 40%;
            h2 {
                transition: all 0.8s ease-out;
            }
        }
       
        .object-3d {
            position: absolute;
            width: 100%;
            height: 100vh;
            .purple-base {
            position: absolute;
            right: 0%;
            width: 93%;
            top: 54.8%;
        }
        .yellow-rectangle {
            position: absolute;
            right: 13.5%;
            top: 63%;
            width: 22%;
        }
        .blue-block {
            position: absolute;
            width: 30%;
            top: 62.5%;
            right: 45%;
        }
        .purple-light-block {
            position: absolute;
            right: 30%;
            top: 50%;
            width: 28%;
        }
        .pink-block {
            position: absolute;
            width: 13.5%;
            right: 37%;
            top: 49%;
        }
        .orange-ball {
            position: absolute;
            right: 41%;
            top: 64.5%;
            width: 7%;
        }
        .small-pink-block {
            display: none;
        }
        .white-ball {
            position: absolute;
            right: 4%;
            top: 77%;
            width: 25%;
        }
        .white-block {
            position: absolute;
            width: 25%;
            right: 10%;
            top: 17%;
        }
        .blur-white-block {
            position: absolute;
            width: 25%;
            right: 30%;
            top: 27%;
        }
      
        }
    }
    
    .hero{
        .scroll-down {
            position: absolute;
            bottom: 10%;
            left: 10%;
            z-index: 1;
            .scroll-button {
                width: 60px;
                height: 60px;
                border-radius: 50%;
            }
            .scroll-button-img {
                width: 20px;
                height: 20px;
            }
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }

}
@media screen and (min-width: 640px) {
    .hero {
        background-image: url(../assets/img/bg-main.jpg);
        height: 100vh;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .hero-text {
            position: absolute;
            top: 45%;
            left: 30%;
            width: 43%;
            height: 40%;
            transform: translate(-50%,-50%);
            h2 {
                transition: all 0.8s ease-out;
            }
        }
       
        .object-3d {
            position: absolute;
            width: 100%;
            height: 100vh;
            .purple-base {
            position: absolute;
            right: -5%;
            width: 73%;
            top: 24.8%;
        }
        .yellow-rectangle {
            position: absolute;
            right: 5.5%;
            top: 34.3%;
            width: 17.5%;
        }
        .blue-block {
            position: absolute;
            width: 24%;
            top: 34.2%;
            right: 29.6%;
        }
        .purple-light-block {
            position: absolute;
            right: 19%;
            top: 18%;
            width: 22%;
        }
        .pink-block {
            position: absolute;
            width: 11%;
            right: 24.5%;
            top: 16.5%;
        }
        .orange-ball {
            position: absolute;
            right: 26.5%;
            top: 36%;
            width: 5.5%;
        }
        .small-pink-block {
            position: absolute;
            width: 20%;
            top: 70%;
            right: 38%;
        }
        .white-ball {
            position: absolute;
            right: 4%;
            top: 67%;
            width: 25%;
        }
        .white-block {
            position: absolute;
            width: 25%;
            right: 50%;
            top: 57%;
        }
        .blur-white-block {
            position: absolute;
            width: 25%;
            right: 40%;
            top: 25%;
        }
      
        }
    }
    
    .hero{
        .scroll-down {
            position: absolute;
            bottom: 18%;
            left: 10%;
            z-index: 1;
            .scroll-button {
                width: 60px;
                height: 60px;
                border-radius: 50%;
            }
            .scroll-button-img {
                width: 20px;
                height: 20px;
            }
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }
}


@media screen and (min-width: 768px) {
    .hero {
        background-image: url(../assets/img/bg-main.jpg);
        height: 100vh;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .hero-text {
            position: absolute;
            top: 45%;
            left: 30%;
            width: 43%;
            height: 40%;
            transform: translate(-50%,-50%);
            h2 {
                transition: all 0.8s ease-out;
            }
        }
       
        .object-3d {
            position: absolute;
            width: 100%;
            height: 100vh;
            .purple-base {
            position: absolute;
            right: 2%;
            width: 63%;
            top: 24.8%;
        }
        .yellow-rectangle {
            position: absolute;
            right: 11.1%;
            top: 34.3%;
            width: 15.5%;
        }
        .blue-block {
            position: absolute;
            width: 21%;
            top: 34.2%;
            right: 31.6%;
        }
        .purple-light-block {
            position: absolute;
            right: 21%;
            top: 18%;
            width: 21%;
        }
        .pink-block {
            position: absolute;
            width: 10%;
            right: 26.5%;
            top: 16.5%;
        }
        .orange-ball {
            position: absolute;
            right: 28.5%;
            top: 36%;
            width: 5.5%;
        }
        .small-pink-block {
            position: absolute;
            width: 14%;
            top: 74%;
            right: 43%;
        }
        .white-ball {
            position: absolute;
            right: 4%;
            top: 67%;
            width: 20%;
        }
        .white-block {
            position: absolute;
            width: 20%;
            right: 50%;
            top: 62%;
        }
        .blur-white-block {
            position: absolute;
            width: 20%;
            right: 40%;
            top: 28%;
        }
      
        }
    }
    
    .hero{
        .scroll-down {
            position: absolute;
            bottom: 18%;
            left: 10%;
            z-index: 1;
            .scroll-button {
                width: 80px;
                height: 80px;
                border-radius: 50%;
            }
            .scroll-button-img {
                width: 20px;
                height: 20px;
            }
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }
}


@media screen and (min-width: 1024px) {
    
   .hero{
       .object-3d {
           .purple-base {
           position: absolute;
           right: 5%;
           width: 59%;
           top: 27.8%;
           }
           .yellow-rectangle {
               position: absolute;
               right: 13.2%;
               top: 39.5%;
               width: 14.5%;
           }
           .blue-block {
               position: absolute;
               width: 19.5%;
               top: 39.5%;
               right: 33%;
           }
           .purple-light-block {
               position: absolute;
               right: 23%;
               top: 19%;
               width: 19%;
           }
           .pink-block {
               position: absolute;
               width: 9.6%;
               right: 27.9%;
               top: 16.5%;
           }
           .orange-ball {
               position: absolute;
               right: 30.8%;
               top: 42.5%;
               width: 4.5%;
           }
           .small-pink-block {
               position: absolute;
               width: 14%;
               top: 74%;
               right: 43%;
           }
           .white-ball {
               position: absolute;
               right: 4%;
               top: 67%;
               width: 16%;
           }
           .white-block {
               position: absolute;
               width: 13%;
               right: 50%;
               top: 62%;
           }
           .blur-white-block {
               position: absolute;
               width: 13%;
               right: 40%;
               top: 28%;
           }
        }
        .scroll-down {
            bottom: 12%;
        }
    }
    }
@media screen and (min-width: 1280px) {
    .hero{
            .scroll-down {
                bottom: 5%;
            }
        }
    }
@media screen and (min-width: 1440px) {
    .hero{
       .object-3d {
           .purple-base {
           position: absolute;
           right: 3%;
           width: 59%;
           top: 20%;
           }
           .yellow-rectangle {
               right: 11.3%;
               top: 37.9%;
               width: 13.5%;
           }
           .blue-block {
               position: absolute;
               width: 19.5%;
               top: 36.7%;
               right: 31%;
           }
           .purple-light-block {
               position: absolute;
               right: 22.5%;
               top: 15%;
               width: 17%;
           }
           .pink-block {
               position: absolute;
               width: 8.5%;
               right: 26.8%;
               top: 12.5%;
           }
           .orange-ball {
               position: absolute;
               right: 29%;
               top: 40%;
               width: 4.5%;
           }
           .small-pink-block {
               position: absolute;
               width: 14%;
               top: 74%;
               right: 43%;
           }
           .white-ball {
               position: absolute;
               right: 4%;
               top: 67%;
               width: 16%;
           }
           .white-block {
               position: absolute;
               width: 13%;
               right: 50%;
               top: 62%;
           }
           .blur-white-block {
               position: absolute;
               width: 13%;
               right: 40%;
               top: 28%;
           }
        }
    }
    }
    </style>
    

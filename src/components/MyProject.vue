<script setup lang="ts">
import type { Page } from '@/Interfaces/type';

const props = defineProps<{
    page: Page
}>()
const emit = defineEmits<{
    (e: 'navigate', page : Page) : void ;
}>()
</script>

<template>
    <div class="project pt-20 pb-40">
        <div class="content-project">
            <div class="project-text flex flex-col justify-around mb-10">
                <h5 v-motion-slide-visible-bottom class="animation-05 text-2xl">Thibault Garcia</h5>
                <h2 v-motion-slide-visible-bottom
                 class="text-2xl sm:text-5xl font-semibold animation-05">Jetez un coup d'oeil à mon projet.</h2>
            </div>
            <div  class="presentation-project">
                <div class="boutique shadow-xl">
                    <div class="top-boutique flex justify-center items-center">
                        <div v-motion-slide-visible-bottom class="picture-boutique animation-05">
                            <img class="picture" src="../assets/img/Home-e-commerce.png" alt="">
                        </div>
                    </div>
                    <div class="bottom-boutique flex justify-center items-center">
                        <div class="text-bottom  text-center">
                            <h3 v-motion-slide-visible-bottom class="text-2xl sm:text-4xl font-semibold animation-05">Boutique E-commerce</h3>
                            <h5 v-motion-slide-visible-bottom class="text-lg animation-05">Projet fictif</h5>
                        </div>
                    </div>
                </div>
            </div>
            <div class="picture-back">
                <img v-motion-slide-visible-right class="pink-block animation-07" src="../assets/img/main-pic-1.png" alt="pink-block">
                <img v-motion-slide-visible-left class="white-block animation-07" src="../assets/img/figure-2.png" alt="pink-block">
                <img v-motion-slide-visible-bottom
                class="white-block-1 animation-07" src="../assets/img/figure-2.png" alt="white-block">
            </div>
        </div>
       
</div>
</template>
    
<style scoped lang="scss">
@media screen and (max-width: 640px) {
    .project {
    background-color: #f1f3f4;
    position: relative;
    z-index: 1;
}
    .content-project {
        width: 90%;
        margin: auto;
        .project-text {
        height: 200px;
        width: 80%;
       z-index: 1000;
    }
    .boutique {
        border-radius: 0px 0px 24px 24px;
    }
    .presentation-project {
        width: 90%;
        margin: auto;
        .top-boutique {
            background-image: url(../assets/img/background-project-2.jpg);
            background-size: cover;
            height: 100%;
            border-radius: 24px 24px 0px 0px;
        }
        .bottom-boutique {
            height: 150px;
            border-radius: 0px 0px 24px 24px;
        }
        .picture-boutique {
            width: 90%;
            height: 85%;
        }
        .picture {
            width: 100%;
            height: 100%;
            border-radius: 24px;
        }
       
    }
    .picture-back {
            position: relative;
            .pink-block {
            position: absolute;
            top: -600px;
            left: -20%;
            z-index: -1;
            width: 250px;
        }
        .white-block {
            display: none;
        }
        .white-block-1 {
            display: none;
        }
        }
    }
}
@media screen and (min-width: 640px) {
    .project {
    background-color: #f1f3f4;
    position: relative;
    z-index: 1;
}
    .content-project {
        width: 90%;
        margin: auto;
        .project-text {
        height: 200px;
        width: 467px;
       z-index: 1000;
    }
    .boutique {
        border-radius: 0px 0px 24px 24px;
    }
    .presentation-project {
        width: 90%;
        margin: auto;
        .top-boutique {
            background-image: url(../assets/img/background-project-2.jpg);
            background-size: cover;
            height: 450px;
            border-radius: 24px 24px 0px 0px;
        }
        .bottom-boutique {
            height: 150px;
            border-radius: 0px 0px 24px 24px;
        }
        .picture-boutique {
            width: 90%;
            height: 85%;
        }
        .picture {
            width: 100%;
            height: 100%;
            border-radius: 24px;
        }
       
    }
    .picture-back {
            position: relative;
            .pink-block {
            position: absolute;
            top: -800px;
            left: -20%;
            z-index: -1;
            width: 300px;
        }
        .white-block {
            position: absolute;
            top: -840px;
            left: 35%;
            width: 27%;
        }
        .white-block-1 {
            display: none;
        }
        }
    }
}
@media screen and (min-width: 768px) {
    .project {

        .content-project{
            .presentation-project {
                width: 90%;
                margin: auto;
            }
            .presentation-project{
                .top-boutique {
                    height: 350px;
                }
            }
            .picture-back {
                    .pink-block {
                    width: 300px;
                }
                .white-block-1{
                    left: -14%;
                }
               
            }
        }
    }
    
}
@media screen and (min-width: 1024px) {
    .project{

        .content-project{
            .presentation-project {
                width: 80%;
                margin: auto;
            }
            .presentation-project{
                .top-boutique {
                    height: 400px;
                }
            }
        }
        .picture-back {
                .pink-block {
                width: 450px;
                .white-block-1 {
                top: -340px;
                left: 0%;
                width: 19%;
            }
            }
        }
    }
}
@media screen and (min-width: 1280px) {
    .project{
        .content-project{
            .presentation-project {
                width: 70%;
                margin: auto;
            }
            .presentation-project {
                .top-boutique {
                    height: 500px;
                }
            }
        }

    }
}

   
</style>
    

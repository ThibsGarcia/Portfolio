<script setup lang="ts">
import MesPassions from '../Features/MesPassions.vue';
import WorkTogether from '../Features/WorkTogether.vue';
import IWork from './IWork.vue';


</script>

<template>
    <section>
        <div class="hero-about pt-20">
            <div class="content-hero flex justify-around">
                <div class="hero-left flex flex-col justify-around">
                    <h3 v-motion
                        :initial="{ opacity: 0, y: 100 }"
                        :enter="{ opacity: 1, y: 0, scale: 1 }"
                        :variants="{ custom: { scale: 2 } }"
                        :delay="100" 
                    class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl xl:text-6xl animation-07 font-semibold">Hey, je suis Thibault Garcia,Front-end Développeur.</h3>
                    <h3 v-motion
                        :initial="{ opacity: 0, y: 100 }"
                        :enter="{ opacity: 1, y: 0, scale: 1 }"
                        :variants="{ custom: { scale: 2 } }"
                        :delay="300"
                    class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl xl:text-6xl animation-07 font-semibold">Originaire de la Côte Basque.</h3>
                </div>
                <div class="hero-right">
                    <div v-motion
                        :initial="{ opacity: 0, x: 100 }"
                        :enter="{ opacity: 1, x: 0, scale: 1 }"
                        :variants="{ custom: { scale: 2 } }"
                        :delay="200"
                    
                    class="right-picture flex justify-center animation-07">
                        <img class="shadow-slate-700" src="../assets/img/photo-thibault.jpg" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
    <IWork/>
    <div class="conten-passion">
        <div class="passion flex justify-around pb-20">
            <MesPassions/>
        </div>
    </div>
    <WorkTogether/>
</template>

<style scoped lang="scss">
@media screen and (max-width: 640px) {
    
    .hero-about {
   height: 100vh;
   background-image: url(../assets/img/back-about.jpg);
   background-size: cover;
    .content-hero {
        height: 80%;
        width: 100%;
        margin: auto;
        flex-direction: column;
        .hero-left, .hero-right {
            margin: auto;
            width: 80%;
            height: 50%;
            color: white;
        }
        .hero-right{
            height: 80%;
            width: 48%;
            margin: auto;
            .right-picture{
                height: 100%;
                display: flex;
                align-items: center;
                img {
                    height: 70%;
                   border-radius: 50%;
                }
            }
        }
    }
}
.conten-passion{
    .passion {
        width: 80%;
        margin: auto;
    }
}
}
@media screen and (min-width: 640px) {
    .hero-about {
   height: 100vh;
   background-image: url(../assets/img/back-about.jpg);
   background-size: cover;
    .content-hero {
        height: 80%;
        width: 80%;
        margin: auto;
        .hero-left, .hero-right {
            margin: auto;
            width: 48%;
            height: 70%;
            color: white;
        }
        .hero-right{
            height: 80%;
            width: 48%;
            margin: auto;
            .right-picture{
                height: 100%;
                display: flex;
                align-items: center;
                img {
                    height: 70%;
                   border-radius: 50%;
                }
            }
        }
    }
}
.conten-passion{
    .passion {
        width: 80%;
        margin: auto;
    }
}
}
@media screen and (min-width: 768px) {
    .hero-about {
   height: 100vh;
   background-image: url(../assets/img/back-about.jpg);
   background-size: cover;
    .content-hero {
        height: 80%;
        width: 80%;
        margin: auto;
        .hero-left, .hero-right {
            margin: auto;
            width: 48%;
            height: 70%;
            color: white;
        }
        .hero-right{
            height: 80%;
            width: 48%;
            margin: auto;
            .right-picture{
                height: 100%;
                display: flex;
                align-items: center;
                img {
                    height: 70%;
                   border-radius: 50%;
                }
            }
        }
    }
}
.conten-passion{
    .passion {
        width: 80%;
        margin: auto;
    }
}
}
@media screen and (min-width: 1024px) {
    .hero-about {
    .content-hero {
        height: 80%;
        width: 80%;
        margin: auto;
        .hero-left, .hero-right {
            margin: auto;
            width: 48%;
            height: 70%;
            color: white;
        }
        .hero-right{
            height: 80%;
            width: 48%;
            margin: auto;
            .right-picture{
                height: 100%;
                display: flex;
                align-items: center;
                img {
                    height: 80%;
                }
            }
        }
    }
}
.conten-passion{
    background-color:#f2f4f5 ;
    .passion {
        width: 80%;
        margin: auto;
    }
}
}
@media screen and (min-width: 1280px) {
    .hero-about {
    .content-hero {
        height: 80%;
        width: 80%;
        margin: auto;
        .hero-left, .hero-right {
            margin: auto;
            width: 48%;
            height: 70%;
            color: white;
        }
        .hero-right{
            height: 80%;
            width: 48%;
            margin: auto;
            .right-picture{
                height: 100%;
                img {
                    height: 100%;
                }
            }
        }
    }
}
.conten-passion{
    background-color:#f2f4f5 ;
    .passion {
        width: 80%;
        margin: auto;
    }
}

}
</style>

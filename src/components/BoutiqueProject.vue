<script setup lang="ts">
import WorkTogetherVue from '../Features/WorkTogether.vue';
import TheCube from '@/Features/Cube.vue'


</script>

<template>
<section>
    <div class="title flex items-center">
        <div class="title-content flex items-center justify-around">
            <div class="left-title flex flex-col justify-around">
                <h5 v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="200"
                class="text-xl font-semibold animation-05">E-commerce shop</h5>
                <h2 v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="400"
                class="text-2xl sm:text-3xl md:text-4xl lg:text-6xl xl:text-7xl font-semibold animation-05">Boutique en ligne</h2>
                <p v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="600"
                class="text-xl animation-05">Ce projet met en avant l'ensemble des technologies que je maîtrise et mes capacités de développement.</p>
            </div>
            <div class="right-title">
                <div class="right-text">
                    <h3 v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :hovered="{ scale: 1.02 }"
                    :delay="400"
                    class="text-center text-xl md:text-2xl lg:text-3xl animation-07">Programmation: Langages/Frameworks</h3>
                </div>
                <TheCube />
            </div>
        </div>
    </div>
    <article>
        <div 
        class="presentation-boutique">
            <img v-motion
                    :initial="{ opacity: 0, y: 200 }"
                    :enter="{ opacity: 1, y: 0, scale: 1 }"
                    :delay="800"
                    :hovered="{ scale: 1}"
            class="boutique-back animation-07" src="../assets/img/boutiqueproject/image-best-gear.jpg" alt="boutique-project">
            <div class="hero-boutique">
                <img v-motion-slide-visible-bottom
                class="hero-picture rounded-2xl animation-07" src="../assets/img/boutiqueproject/hero.png" alt="boutique-project">
            </div>
        </div>
    </article>
    <article>
        <div class="description flex">
            <div class="content-description flex justify-around">
                <div class="left-description flex flex-col justify-around items-center ">
                    <div>
                        <h4 v-motion-slide-visible-bottom
                        class="text-xl lg:text-4xl font-semibold mt-5 animation-07">Vue d'ensemble</h4>
                    </div>
                    <div>
                        <button v-motion-slide-visible-bottom class="animation-07"><a href="https://laxai-shop.com/" target="_blank">Ouvrir Site</a></button>
                    </div>
                </div>
                <div class="right-description flex flex-col justify-between">
                    <div class="top-right-description">
                        <p v-motion-slide-visible-bottom
                        class="lg:text-xl xl:text-2xl animation-07">Le projet e-commerce est un challenge du site Frontend Mentor. <br>Il s'agit de mon projet le plus abouti, mettant en avant l'ensemble de mes compétences.</p>
                    </div>
                    <div class="down-right-description">
                        <p v-motion-slide-visible-bottom
                        class="lg:text-xl xl:text-2xl animation-07">Durant ma formation, j'ai appris à créer une page d'un site e-commerce réactif. Cependant, pour aller plus loin  et complexifier le projet, j'ai décidé de développer un site complet.</p>
                    </div>
                </div>
            </div>
        </div>
    </article>
  

    <article>
        <div class="galerie-boutique pb-20">
            <div class="galerie-content">
                <div v-motion-slide-visible-bottom
                class="galerie-content pt-10">
                    <img v-motion-slide-visible-bottom class="rounded-2xl animation-05"
                    src="../assets/img/boutiqueproject/product-facing.png" alt="galerie-boutique">
                </div>
                <div class="pt-10 flex justify-around items-center">
                    <div class="galerie-content-3">
                        <img v-motion-slide-visible-bottom class="rounded-2xl animation-05"
                        src="../assets/img/boutiqueproject/also-like.png" alt="boutique-project">
                    </div>
                    <div class="galerie-content-3">
                        <img v-motion-slide-visible-bottom class="rounded-2xl animation-05"
                        src="../assets/img/boutiqueproject/homePage.png" alt="boutique-project">
                    </div>
                </div>
                <div class="galerie-content flex justify-end pt-10">
                    <img v-motion-slide-visible-bottom 
                    class="picture-content rounded-2xl animation-05" src="../assets/img/boutiqueproject/product-description.png" alt="galerie-boutique">
                </div>
                <div class="pt-10 flex justify-around">
                    <div class="galerie-content-3">
                        <img v-motion-slide-visible-bottom class="rounded-2xl animation-05"
                        src="../assets/img/boutiqueproject/Order.png" alt="galerie-boutique">
                    </div>
                    <div class="galerie-content-3 flex items-center">
                        <img v-motion-slide-visible-bottom class="rounded-2xl animation-05"
                        src="../assets/img/boutiqueproject/mini-cart.png" alt="galerie-boutique">
                    </div>
                </div>
            </div>
        </div>
    </article>
</section>
<WorkTogetherVue/>

</template>

<style scoped lang="scss">
@media screen and (max-width: 640px) {
    .title {
    height: 85vh;
}
.title-content {
    width: 90%;
    margin: auto;
    height: 80%;
    display: flex;
    flex-direction: column;
}
.left-title {
    width: 60%;
    height: 35%;
}
.right-title {
    height: 45%;
    width: 100%;
}
.top-right {
    height: 25%;
}
.right-down {
    height: 75%;
    img {
        width: 50px;
        height: 50px;
    }
}

.presentation-boutique {
    width: 100%;
    background-color:#f2f4f5;
    .boutique-back {
        width: 100%;
    }
    .hero-boutique {
        .hero-picture {
            position: relative;
            top: -150px;
            height: 50%;
            width: 80%;
            margin: auto;
        }
    }
}

.description {
    height: 60vh;
    .content-description {
        width: 80%;
        height: 90%;
        margin: auto;
        flex-direction: column;
        .left-description {
        width: 100%;
        height: 40%;
        }
        .right-description {
            width: 100%;
            height: 50%;
        }
        button {
            width: 150px;
            height: 40px;
            background-color: #d87d4a;
            border-radius: 14px;
        }
    }
}

.home-page-also {
    height: 80vh;
    .home-page-content{
        height: 100%;
        width: 40%;
        margin: auto;
        .home-page-picture {
            height:90%;
        }
        
    } 
}

.galerie-boutique {
    background-color:#f2f4f5;
    .galerie-content {
        width: 80%;
        margin: auto;
    }
    .galerie-content-3 {
        width: 45%;
    }
    .galerie-content-4 {
        width: 80%;
        margin: auto;
        .picture-content{
            height: 80vh;
        }
    }
}

}
@media screen and (min-width: 640px) {
    
.title {
    height: 85vh;
}
.title-content {
    width: 75%;
    margin: auto;
    height: 90%;
}
.left-title {
    width: 60%;
    height: 65%;
}
.right-title {
    height: 50%;
    width: 25%;
}
.top-right {
    height: 25%;
}
.right-down {
    height: 75%;
    img {
        width: 50px;
        height: 50px;
    }
}

.presentation-boutique {
    width: 100%;
    background-color:#f2f4f5;
    .boutique-back {
        width: 100%;
    }
    .hero-boutique {
        .hero-picture {
            position: relative;
            top: -150px;
            height: 50%;
            width: 80%;
            margin: auto;
        }
    }
}

.description {
    height: 60vh;
    .content-description {
        width: 80%;
        height: 65%;
        margin: auto;
        .left-description {
        width: 30%;
        height: 70%;
        }
        .right-description {
            width: 60%;
        }
        button {
            width: 150px;
            height: 40px;
            background-color: #d87d4a;
            border-radius: 14px;
        }
    }
}

.home-page-also {
    height: 80vh;
    .home-page-content{
        height: 100%;
        width: 40%;
        margin: auto;
        .home-page-picture {
            height:90%;
        }
        
    } 
}

.galerie-boutique {
    background-color:#f2f4f5;
    .galerie-content {
        width: 80%;
        margin: auto;
    }
    .galerie-content-3 {
        width: 45%;
    }
    .galerie-content-4 {
        width: 80%;
        margin: auto;
        .picture-content{
            height: 80vh;
        }
    }
}

}
@media screen and (min-width: 768px) {
    .title{
        .title-content {
        width: 90%;
        height: 80%;
        }
        .right-title{
            width: 35%;
        }
    }
}
@media screen and (min-width: 1024px) {
    .title-content {
    width: 85%;
    margin: auto;
    height: 90%;
    }
    .left-title {
        width: 50%;
        height: 65%;
    }
    .right-title {
        height: 50%;
        width: 35%;
    }
    .description{
        .content-description{
            .left-description {
                width: 40%;
                height: 90%;
            }
            .right-description{
                width: 50%;
            }
        }
    }
}
@media screen and (min-width: 1280px) {
    .title{
        .title-content {
        width: 75%;
        margin: auto;
        height: 90%;
        }
        .left-title {
            width: 60%;
            height: 65%;
        }
        .right-title {
            height: 50%;
            width: 25%;
        }
    }
}

</style>

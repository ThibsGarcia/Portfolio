<script setup lang="ts">

</script>

<template>
<div class="work-with flex">
    <div class="content-work">
        <div class="text-work flex flex-col justify-around">
            
            <div class="bottom-content flex flex-col  justify-around">
                <h4 v-motion-slide-visible-bottom class="text-lg sm:text-xl animation-07">Je suis un jeune développeur du Pays Basque, passionné par le monde de la technologie.</h4>
                <p v-motion-slide-visible-bottom class="text-lg sm:text-xl animation-07">Je suis une personne très curieuse et avide de connaissances, cherchant toujours à approfondir mes compétences, que ce soit dans ma vie professionnelle ou personnelle.</p>
                <p v-motion-slide-visible-bottom class="text-lg sm:text-xl animation-07">Je suis convaincu que ce domaine offre un potentiel infini pour mon développement, et je suis impatient à l'idée de continuer à apprendre et à progresser dans cette industrie en constante évolution.</p>
            </div>
            <div v-motion-slide-visible-bottom class="scroll-down flex items-center animation-07">
                <div  
                class="scroll-button flex justify-center items-center shadow-2xl mr-5 ">
                    <img class="scroll-button-img" src="../assets/img/scroll.svg" alt="scroll-button">
                </div>
                 <h6>Scroll</h6>
            </div>
        </div>
        
    </div>
    <div class="object-work">
        <img class="pattern-circles" src="../assets/img/pattern-circles.svg" alt="pattern-circle">
        <img v-motion-slide-visible-bottom class="orange-ball animation-07" src="../assets/img/work-cube-4.png" alt="orange-ball">
        <img v-motion-slide-visible-left class="pink-block-top animation-07" src="../assets/img/work-cube-1.png" alt="orange-ball">
        <img v-motion-slide-visible-bottom class="white-ball animation-07" src="../assets/img/work-cube-2.png" alt="white-ball">
        <img v-motion-slide-visible-bottom class="white-blur-ball animation-07" src="../assets/img/work-cube-3.png" alt="white-ball">
        <img v-motion-slide-visible-bottom class="pink-block-1 animation-07" src="../assets/img/work-cube-6.png" alt="pink-block">
        <img v-motion-slide-visible-bottom class="pink-block-2 animation-07" src="../assets/img/work-cube-6.png" alt="pink-block">
        <img v-motion-slide-visible-left class="purple-block animation-07" src="../assets/img/work-cube-7.png" alt="purple-block">
    </div>

</div>

</template>

<style scoped lang="scss">
@media screen and (max-width: 640px) {
    .work-with {
    background-color: #1B1B87;
    height: 100vh;
    width: 100%;
    .content-work {
        width: 80%;
    }
    .object-work{
        width: 60%;
    }
  
    .text-work {
        position: relative;
        justify-content: space-between;
        width: 100%;
        height: 70%;
        top: 5%;
        left: 10%;
    }
   
    .bottom-content {
        color: white;
        height: 80%;
    }
    .object-work {
     position: absolute;   
    }
    .orange-ball {
        position: absolute;
        left: 3%;
        top: 520px;
    }
    .pink-block-top {
        position: absolute;
        top: 450px;
        left: 10%;
    }
    .white-ball {
        position: absolute;
        top: 540px;
        left: 35%;
    }
    .white-blur-ball {
        position: absolute;
        top: 500px;
        left: -10%;
    }
    .pink-block-1 {
        position: absolute;
        top: 390px;
        left: -14%;
    }
    .pink-block-2 {
        position: absolute;
        top: 420px;
        left: 25%;
    }
    .purple-block {
        position: absolute;
        top: 530px;
        left: 15%;
    }
   
    .pattern-circles {
        position: absolute;
        left: 30%;
        top: 450px;
        width: 90%;
    }
}
.scroll-down {
        color: white;
        .scroll-button {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: white;
        }
        .scroll-button-img {
            width: 20px;
            height: 20px;
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }
}
@media screen and (min-width: 640px) {
    .work-with {
    background-color: #1B1B87;
    height: 100vh;
    width: 100%;
    .content-work {
        width: 50%;
    }
    .object-work{
        width: 60%;
    }
  
    .text-work {
        position: relative;
        width: 100%;
        height: 100%;
        top: 50%;
        left: 50%;
        transform: translate(-40%, -50%);
    }
   
    .bottom-content {
        color: white;
        height: 70%;
    }
    .object-work {
     position: absolute;   
    }
    .orange-ball {
        position: absolute;
        left: 45%;
        top: 280px;
    }
    .pink-block-top {
        position: absolute;
        top: 170px;
        left: 50%;
    }
    .white-ball {
        position: absolute;
        top: 290px;
        left: 45%;
    }
    .white-blur-ball {
        position: absolute;
        top: 290px;
        left: 59%;
    }
    .pink-block-1 {
        position: absolute;
        top: 140px;
        left: 28%;
    }
    .pink-block-2 {
        position: absolute;
        top: 150px;
        left: 65%;
    }
    .purple-block {
        position: absolute;
        top: 290px;
        left: 59%;
    }
   
    .pattern-circles {
        position: absolute;
        left: 65%;
        top: 150px;
    }
}
.scroll-down {
        color: white;
        .scroll-button {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: white;
        }
        .scroll-button-img {
            width: 20px;
            height: 20px;
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }
}
@media screen and (min-width: 768px) {
    .work-with {
    background-color: #1B1B87;
    height: 100vh;
    width: 100%;
    .content-work {
        width: 50%;
    }
    .object-work{
        width: 60%;
    }
  
    .text-work {
        position: relative;
        width: 100%;
        height: 100%;
        top: 50%;
        left: 50%;
        transform: translate(-40%, -50%);
    }
    .bottom-content {
        color: white;
        height: 70%;
    }
    .object-work {
     position: absolute;   
    }
    .orange-ball {
        position: absolute;
        left: 45%;
        top: 280px;
    }
    .pink-block-top {
        position: absolute;
        top: 170px;
        left: 50%;
    }
    .white-ball {
        position: absolute;
        top: 310px;
        left: 45%;
    }
    .white-blur-ball {
        position: absolute;
        top: 310px;
        left: 59%;
    }
    .pink-block-1 {
        position: absolute;
        top: 140px;
        left: 28%;
    }
    .pink-block-2 {
        position: absolute;
        top: 150px;
        left: 65%;
    }
    .purple-block {
        position: absolute;
        top: 290px;
        left: 59%;
    }
   
    .pattern-circles {
        position: absolute;
        left: 65%;
        top: 150px;
    }
}
.scroll-down {
        color: white;
        .scroll-button {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: white;
        }
        .scroll-button-img {
            width: 20px;
            height: 20px;
        }
    }
    .scroll-button:hover {
        box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
        transform: scale(1.1);
    }
}
@media screen and (min-width: 1024px) {
    .work-with{
        .content-work, .object-work {
        width: 50%;
    }
    .text-work {
        position: relative;
        width: 80%;
        height: 80%;
        top: 50%;
        left: 50%;
        transform: translate(-40%, -50%);
    }
        .object-work {
         position: absolute;  
            .orange-ball {
                left: 76%;
                top: 280px;
            }
            .pink-block-top {
                top: 190px;
                left: 84%;
            }
            .white-ball {
                top: 280px;
                left: 75%;
            }
            .white-blur-ball {
                top: 350px;
                left: 89%;
            }
            .pink-block-1 {
                top: 120px;
                left: 61%;
            }
            .pink-block-2 {
                top: 160px;
                left: 97%;
            }
            .purple-block {
                top: 300px;
                left: 90%;
            }
        
            .pattern-circles {
                position: absolute;
                left: 100%;
                bottom: -600px;
                width: 100%;
                } 
        }
        
    }

}
@media screen and (min-width: 1280px) {
    .work-with{
        .object-work {
         position: absolute;   
            .orange-ball {
                left: 76%;
                top: 220px;
            }
            .pink-block-top {
                top: 80px;
                left: 84%;
            }
            .white-ball {
                top: 540px;
                left: 70%;
            }
            .white-blur-ball {
                top: 320px;
                left: 89%;
            }
            .pink-block-1 {
                top: -50px;
                left: 61%;
            }
            .pink-block-2 {
                top: 0px;
                left: 97%;
            }
            .purple-block {
                top: 220px;
                left: 90%;
            }
            .pattern-circles {
                right: 0%;
                top: 10px;
            }
        }
    }
}


</style>

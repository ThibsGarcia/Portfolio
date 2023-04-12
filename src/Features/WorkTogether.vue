<script setup lang="ts">

</script>

<template>
<div class="container-work flex mb-10">
    <div class="content flex flex-col space-around">
        <div class="top-content flex">
            <div class="text-content">
                <div class="text flex flex-col justify-around pt-20">
                    <h5 v-motion-slide-visible-bottom class="text-2xl animation-05">Contact</h5>
                    <h2 v-motion-slide-visible-bottom class="text-3xl md:text-5xl font-semibold animation-05">Unissons nos forces</h2>
                    <p v-motion-slide-visible-bottom class="text-lg">Je serais ravi de vous rencontrer pour discuter de votre projet et d'éventuelles collaborations.</p>
                </div>
            </div>
                <div class="object-3d">
                    <img v-motion-slide-visible-bottom   class="purple-base animation-05" src="../assets/img/figures-1.png" alt="object-3d">
                    <img v-motion-slide-visible-right   class="blue-block animation-05" src="../assets/img/figures-3.png" alt="object-3d">
                    <img v-motion-slide-visible-left   class="yellow-rectangle animation-05" src="../assets/img/figures-4.png" alt="object-3d">
                    <img v-motion-slide-visible-bottom   class="orange-ball animation-05" src="../assets/img/figures-2.png" alt="object-3d">
                    <img v-motion-slide-visible-bottom   class="white-ball animation-05" src="../assets/img/figures-5.png" alt="object-3d">
                    <img v-motion-slide-visible-bottom   class="white-ball-big animation-05" src="../assets/img/figures-6.png" alt="object-3d">
                </div>
        </div>
        <div class="contact-content flex justify-between pt-20 xl:pt-60">
            <div class="">
                <div class="text-information flex flex-col justify-between">
                    <div v-motion-slide-visible-bottom class="text-bloc-info flex items-center animation-05">
                        <img class="mr-10 w-8" src="../assets/icons/email.svg" alt="icon">
                        <h5 class="text-lg lg:text-3xl">thibaultgarcia.64@gmail.com</h5>
                    </div>
                    <div v-motion-slide-visible-bottom class="text-bloc-info flex items-center animation-05">
                        <img class="mr-10 w-8" src="../assets/icons/place.svg" alt="icon">
                        <h5 class="text-lg lg:text-3xl">Ascain, Pays Basque, France</h5>
                    </div>
                    <div v-motion-slide-visible-bottom class="text-bloc-info flex items-center animation-05">
                        <img class="mr-10 w-8" src="../assets/icons/phone.svg" alt="icon">
                        <h5 class="text-lg lg:text-3xl"> 06 65 55 83 47</h5>
                    </div>
                </div>
            </div>
            <div class="talk">
                <div class="content-talk">
                    <form class="formulaire flex flex-col justify-between" action="#">
                        <div v-motion-slide-visible-bottom class="input animation-05">
                            <input class="input-1 pl-5" type="text" required placeholder="Name">
                        </div>
                        <div v-motion-slide-visible-bottom class="input animation-05">
                            <input class="input-1 pl-5" type="email" required placeholder="Email">
                        </div>
                        <div v-motion-slide-visible-bottom class="input animation-05">
                            <input class="input-2 pl-5" type="text" name="message" id="message" placeholder="Attention je ne suis pas fonctionnel.">
                        </div>
                        <div v-motion-slide-visible-bottom class="btn-1 animation-03">
                            <button class="text-lg" type="submit">Envoyer</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
        <div class="reseaux flex justify-around">
                <div v-motion-slide-visible-bottom  class="icone flex items-center justify-center animation-03">
                    <img class="logo mr-5" src="../assets/icons/linkedin.png" alt="linkedin">
                    <a href="https://www.linkedin.com/in/thibault-garcia-461b35161/" target="_blank" rel="noopener noreferrer"><h5>linkedin</h5></a>
                </div>
                <div v-motion-slide-visible-bottom  class="icone flex items-center justify-center animation-03">
                    <img class="logo mr-5" src="../assets/icons/linkedin.png" alt="linkedin">
                    <a href="https://www.linkedin.com/in/thibault-garcia-461b35161/" target="_blank" rel="noopener noreferrer"><h5>linkedin</h5></a>
                </div>
            </div>
    </div>
    <div class="back-elipse"></div>
</div>
</template>

<style lang="scss">
@media screen and (max-width: 640px) {
    .container-work {
    background-color: #f1f3f4;
}
.content {
    z-index: 1;
    width: 100%;
    height: 230vh;
    background-color: #ffffff;
    margin: auto;
    .contact-content{
        display: flex;
        flex-direction: column;
        height: 80%;
    }    
    .text-content {
        width: 90%;
        margin: auto;
        .text {
            width: 70%;
            height: 357px;
        }
    }

    .object-3d {
        position: absolute;
        width: 90%;
        height: 100vh;

        .purple-base {
        position: absolute;
        right: -10%;
        top: 20%;
        width: 90%;
    }
    .yellow-rectangle {
        position: absolute;
        right: 3%;
        top: 23.5%;
        width: 20%;
    }
    .blue-block {
        position: absolute;
        top: 18%;
        right: 3%;
        width: 16%;
    }
    .orange-ball {
        position: absolute;
        right: -4%;
        top: 14%;
        z-index: 1;
    }
    .white-ball {
        display: none;

    }
    .white-ball-big {
        display: none;
    }
    }
    .text-information {
        width: 80%;
        margin: auto;
        height: 244px;
        margin-bottom: 50px;
    }
    .talk {
        .content-talk, .formulaire {
        width: 90%;
        margin: auto;
        height: 592px;
        z-index: 1;
        }
        .input-box {
            width: 98%;
        }
        .input-1 {
            width: 100%;
            height: 72px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2 {
            position: relative;
            width: 100%;
            height: 200px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2::placeholder {
            transform: translateY(-250%);
        }

        .input-1:hover, .input-2:hover{
            border: 2px solid blue;
            color: black;
        }
        button {
            width: 100%;
            height: 72px;
            background-color: #4C40F7;
            color: white;
            border-radius: 20px;
        }
    }
    .reseaux {
        width: 80%;
        margin: auto;
        .icone {
            width: 25%;
            height: 120px;
            border-radius: 24px;
            z-index: 3;
        }
        .logo {
            height: 20%;
            }
        .icone:hover {
            box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
            transform: scale(1.1);
        }
    }
}
.back-elipse {
    position: absolute;
    width: 100%;
    height: 1360px;
    background-color: #00113B;
    clip-path: ellipse(1300px 840px at 75% 70%);
    z-index: 0;
        }

}

@media screen and (min-width: 640px) {
    .container-work {
    background-color: #f1f3f4;
}
.content {
    z-index: 1;
    width: 80%;
    height: 180vh;
    background-color: #ffffff;
    margin: auto;
    border-radius: 24px;
    box-shadow: rgba(240, 46, 170, 0.4) 5px 5px, rgba(240, 46, 170, 0.3) 10px 10px, rgba(240, 46, 170, 0.2) 15px 15px, rgba(240, 46, 170, 0.1) 20px 20px, rgba(240, 46, 170, 0.05) 25px 25px;
    .contact-content{
        display: flex;
        flex-direction: column;
        height: 80%;
    }    
    .text-content {
        width: 90%;
        margin: auto;
        .text {
            width: 50%;
            height: 357px;
        }
    }

    .object-3d {
        position: absolute;
        width: 90%;
        height: 100vh;

        .purple-base {
        position: absolute;
        right: 1%;
        top: 11%;
        width: 90%;
    }
    .yellow-rectangle {
        position: absolute;
        right: 13.5%;
        top: 15.5%;
        width: 21%;
    }
    .blue-block {
        position: absolute;
        top: 4.8%;
        right: 18.1%;
        width: 18%;
    }
    .orange-ball {
        position: absolute;
        right: 8%;
        top: -4%;
        z-index: 1;
    }
    .white-ball {
        position: absolute;
        right: 30%;
        top: 36%;
    }
    .white-ball-big {
        position: absolute;
        top: 42%;
        right: 5%;
    }
    }
    .text-information {
        width: 80%;
        margin: auto;
        height: 244px;
    }
    .talk {
        .content-talk, .formulaire {
        width: 90%;
        margin: auto;
        height: 592px;
        z-index: 1;
        }
        .input-box {
            width: 98%;
        }
        .input-1 {
            width: 100%;
            height: 72px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2 {
            position: relative;
            width: 100%;
            height: 200px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2::placeholder {
            transform: translateY(-250%);
        }

        .input-1:hover, .input-2:hover{
            border: 2px solid blue;
            color: black;
        }
        button {
            width: 100%;
            height: 72px;
            background-color: #4C40F7;
            color: white;
            border-radius: 20px;
        }
    }
    .reseaux {
        width: 80%;
        margin: auto;
        .icone {
            width: 25%;
            height: 120px;
            border-radius: 24px;
            z-index: 3;
        }
        .logo {
            height: 20%;
            }
        .icone:hover {
            box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
            transform: scale(1.1);
        }
    }
}
.back-elipse {
    position: absolute;
    width: 100%;
    height: 1360px;
    background-color: #00113B;
    clip-path: ellipse(1300px 840px at 75% 70%);
    z-index: 0;
        }

}
@media screen and (min-width: 768px) {
    .container-work {
    background-color: #f1f3f4;
}
.content {
    z-index: 1;
    width: 80%;
    height: 1213px;
    background-color: #ffffff;
    margin: auto;
    border-radius: 24px;
    box-shadow: rgba(240, 46, 170, 0.4) 5px 5px, rgba(240, 46, 170, 0.3) 10px 10px, rgba(240, 46, 170, 0.2) 15px 15px, rgba(240, 46, 170, 0.1) 20px 20px, rgba(240, 46, 170, 0.05) 25px 25px;
        .text-content, .contact-content {
        display: flex;
        flex-direction: row;
        width: 90%;
        margin: auto;
        .text {
            width: 50%;
            height: 357px;
        }
    }

    .object-3d {
        position: absolute;
        width: 90%;
        height: 100vh;

        .purple-base {
        position: absolute;
        right: 1%;
        top: 11%;
        width: 90%;
    }
    .yellow-rectangle {
        position: absolute;
        right: 13.5%;
        top: 16.5%;
        width: 21%;
    }
    .blue-block {
        position: absolute;
        top: 4.8%;
        right: 16%;
        width: 18%;
    }
    .orange-ball {
        position: absolute;
        right: 8%;
        top: -4%;
        z-index: 1;
    }
    .white-ball {
        position: absolute;
        right: 34%;
        top: 36%;
    }
    .white-ball-big {
        position: absolute;
        top: 42%;
        right: 5%;
    }
    }
    .text-information {
        width: 280px;
        height: 204px;
    }
    .talk {
        .content-talk, .formulaire {
        width: 240px;
        height: 492px;
        z-index: 1;
        }
        .input-box {
            width: 98%;
        }
        .input-1 {
            width: 100%;
            height: 72px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2 {
            position: relative;
            width: 100%;
            height: 200px;
            background-color:#F4F4F4 ;
            color: #6B6B6B;
            border: 1px solid #CFCFCF;
            border-radius: 11px;
        }
        .input-2::placeholder {
            transform: translateY(-250%);
        }

        .input-1:hover, .input-2:hover{
            border: 2px solid blue;
            color: black;
        }
        button {
            width: 242px;
            height: 72px;
            background-color: #4C40F7;
            color: white;
            border-radius: 20px;
        }
    }
    .reseaux {
        width: 80%;
        margin: auto;
        .icone {
            width: 25%;
            height: 120px;
            border-radius: 24px;
            z-index: 3;
        }
        .logo {
            height: 20%;
            }
        .icone:hover {
            box-shadow: rgba(0, 0, 0, 0.09) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
            transform: scale(1.1);
        }
    }
}
.back-elipse {
    position: absolute;
    width: 100%;
    height: 1360px;
    background-color: #00113B;
    clip-path: ellipse(1300px 840px at 75% 70%);
    z-index: 0;
        }
}
@media screen and (min-width: 1024px) {
    .content{
        height: 1313px;
        .talk {
            .content-talk, .formulaire {
            width: 250px;
            height: 492px;
            z-index: 1;
            }
        }
        .object-3d {
                .purple-base {
                right: 1%;
                top: 14%;
                width: 90%;
            }
            .yellow-rectangle {
            right: 14.5%;
            top: 22.5%;
            width: 20%;
            }
            .blue-block {
                position: absolute;
                top: 7%;
                right: 15%;
                width: 17%;
            }
            .orange-ball {
                position: absolute;
                right: 8%;
                top: -4%;
                z-index: 1;
            }
            .white-ball {
            right: 34%;
            top: 40%;
            }
            .white-ball-big {
                top: 49%;
                right: 8%;
            }
        }
    }
}
@media screen and (min-width: 1280px) {
    .content{
        .text-information {
        width: 480px;
        height: 204px;
    }
    .talk {
        .content-talk, .formulaire {
        width: 460px;
        height: 492px;
        z-index: 1;
        }

        }
        .object-3d {
                .purple-base {
                right: 1%;
                top: 11%;
                width: 90%;
            }
            .yellow-rectangle {
            right: 14.3%;
            top: 22.6%;
            width: 20%;
            }
            .blue-block {
                position: absolute;
                top: 4%;
                right: 14.8%;
                width: 15%;
            }
            .orange-ball {
                position: absolute;
                right: 8%;
                top: -4%;
                z-index: 1;
            }
            .white-ball {
            right: 38%;
            top: 45%;
            }
            .white-ball-big {
                top: 52%;
                right: 8%;
            }
        }
    }
    
}



</style>
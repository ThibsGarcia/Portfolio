<script setup lang="ts">

</script>

<template>
<footer>
    <div class="content-footer flex flex-col justify-around">
            <div class="top-content flex flex-col  md:flex-row md:justify-between sm:flex-col">
                <div v-motion-slide-visible-left class="left-part xl:flex xl:items-start xl:justify-center animation-05">
                    <img class="logo" src="../assets/img/LOGO-LAXAA.png" alt="logo-picture">
                </div>
                <div class="center-part flex flex-col items-center justify-around">
                    <h2 v-motion-slide-visible-bottom class="text-4xl sm:text-4xl sm:font-medium md:text-2xl lg:text-4xl xl:text-5xl text-center animation-05">Vous n'avez qu'une seule chance de faire une première impression.</h2>
                    <h5 v-motion-slide-visible-bottom class="text-2xl sm:text-2xl md:text-xl lg:text-2xl xl:text-3xl text-red-300 animation-03">Faisons en sorte qu'elle soit exceptionnelle.</h5>
                </div>
                <div class="right-part flex items-center">
                    <ul v-motion-slide-visible-right class="flex md:flex-col md:justify-around animation-05">
                        <li class="text-base md:text-base lg:text-lg">À propos de moi</li>
                        <li class="text-base md:text-base lg:text-lg">Projet</li>
                        <li class="text-base md:text-base lg:text-lg">Contact</li>
                        <li class="text-base md:text-base lg:text-lg">Linkedin</li>
                    </ul>
                </div>
            </div>
            <div class="bottom flex md:flex-col md:justify-around">
                <div class="ligne">
                </div>
                <div class="bottom-content flex justify-between">
                    <div class="bottom-left">
                        <h5 class="text-base">2020.UI8 LLC.  -  Portfolio 2022</h5>
                    </div>
                    <div class="bottom-right">
                        <h5 class="text-base">Thibault Garcia</h5>
                    </div>
                </div>
            </div>
        </div>
</footer>

</template>

<style scoped lang="scss">
footer {
    background-color: #00113b;
}
.content-footer {
        width: 80%;
        margin: auto;
       color: #ffffff;
}
@media screen and (max-width: 640px) {
    .content-footer{
        height: 85vh;
        flex-direction: column;
    }
    .top-content{
        height: 75%;
        justify-content: space-around;
        .left-part, .right-part, .center-part{
        width: 100%;
        }
        .center-part{
            height: 80%;
            h5 {
                text-align: center;
            }
        }
        .left-part, .right-part{
            height: 15%;
        }
        .logo{
            width: 15%;
        }
        ul{
            justify-content: space-around;
            width: 100%;
        }
    }
    .bottom{
            height: 10%;
            .bottom-content{
                width: 100%;
                margin: auto;
            }
            .ligne {
                height: 1px;
                background-color: #D8D8D8;
            }
        }
}
@media screen and (min-width: 640px) {
    .content-footer{
        height: 85vh;
    }
    .top-content{
        height: 65%;
        .left-part, .right-part, .center-part{
        width: 100%;
        }
        .center-part{
            height: 60%;
        }
        .left-part, .right-part{
            height: 20%;
        }
        .logo{
            width: 12%;
        }
        ul{
            justify-content: space-around;
            width: 100%;
        }
    }
    .bottom{
        height: 20%;
        .bottom-content{
            height: 20%;
            width: 80%;
            margin: auto;
        }
        .ligne {
            height: 1px;
            background-color: #D8D8D8;
        }
    }
}

@media screen and (min-width: 768px) {
    .content-footer{
        height: 45vh;
        width: 90%;
        .top-content {
            height: 65%;
           }
           .center-part{
            width: 60%;
            height: 100%;
           }
           .left-part, .right-part{
            width: 17%;
            height: 90%;
           }
        .bottom {
            width: 90%;
            margin: auto;
            height: 25%;
        }
        .logo{
            width: 55%;
            border-radius: 50%;
        }
        ul{
            height: 60%;
        }
    }
}
@media screen and (min-width: 1024px) {

    .content-footer {
        width: 80%;
        height: 50vh;
        margin: auto;
       color: #ffffff;
       .right-part {
        width: 14%;
       }
        .logo {
         width: 45%;
        }
        ul{
            height: 70%;
        }
       }
}



</style>

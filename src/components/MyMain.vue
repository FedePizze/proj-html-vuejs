<template>
    <div id="main">
        <MainJumbotron></MainJumbotron>
      
        <div id="cardContainerImgCard">
            <div class="row">
                <ImgCard v-for="(elemento, index) in imgArreyRow1" :key="index" :send="elemento"></ImgCard>
                <ShopButton class="pos4"></ShopButton>
                <CircleButton class="pos5"></CircleButton>
            </div>
            <div class="row">
                <ImgCard v-for="(elemento, index) in imgArreyRow2" :key="index" :send="elemento"></ImgCard>
                <ArrowButton class="pos1"></ArrowButton>
                <ArrowButton class="pos3"></ArrowButton>
            </div>
        </div>

        <div class="container">
            <WorkingProcessBox></WorkingProcessBox>
            <ArrowButton class="pos1"></ArrowButton>
        </div>

        <SendMessageBox></SendMessageBox>

        <div class="container">
            <div id="boxEvent">
                <EventCard></EventCard>
            </div>
            
            <ArrowButton class="pos2"></ArrowButton>
        </div>

    </div>
</template>

<script>
import MainJumbotron from "./partials/MainJumbotron.vue"
import ImgCard from "./partials/ImgCard.vue"
import WorkingProcessBox from "./partials/WorkingProcessBox.vue"
import SendMessageBox from "./partials/SendMessageBox.vue"
import EventCard from "./partials/EventCard.vue"

import ArrowButton from "./elements/ArrowButton.vue"
import ShopButton from "./elements/ShopButton.vue"
import CircleButton from "./elements/CircleButton.vue"


export default {
    name: "MyMain" ,
    components: {
        MainJumbotron,
        ImgCard,
        WorkingProcessBox,
        SendMessageBox,
        EventCard,
        ArrowButton,
        ShopButton,
        CircleButton
    },

    data() {
        return{
            imgArreyRow1: [
                {src:"../../../public/img/h-2-port-img-1.jpg"},
                {src:"../../../public/img/h-2-port-img-2.jpg"},
                {src:"../../../public/img/h-2-port-img-3.jpg"}
            ],

            imgArreyRow2: [
                {src:"../../../public/img/h-2-port-img-4.jpg"},
                {src:"../../../public/img/h-2-port-img-5.jpg"},
                {src:"../../../public/img/h-2-port-img-6.jpg"}
            ],

            blogArrey: [
                {
                    src:"../../../public/img/h-2-blog-img-1.jpg",
                    title:"This, way, lover: a detailed guide through new design",
                    author:"Emily Fields",
                    date:"07",
                    month:"MAY",
                    year:"19"
                },
                {
                    src:"../../../public/img/h-2-blog-img-1.jpg",
                    title:"I try to give a people a different way of looking art",
                    author:"Emily Fields",
                    date:"07",
                    month:"MAY",
                    year:"19"
                },
                {
                    src:"../../../public/img/h-2-blog-img-1.jpg",
                    title:"Introduce Richard Lapierrière of those amazing features",
                    author:"Emily Fields",
                    date:"07",
                    month:"MAY",
                    year:"19"
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">

    #cardContainerImgCard{
        width: 100%;

        .row{
            display: flex;
            flex-wrap: wrap;
            position: relative;
        }
    }

    .container{
        position: relative;

        #boxEvent{
            display: flex;
            flex-wrap: wrap;
            width: 60%;
            margin: 0px auto;
            padding: 50px 0px;
        }
    }

    .pos1{
        bottom: 20px;
        right: 20px;
    }

    .pos2{
        top: 20px;
        right: 20px;
    }

    .pos3{
        top: 0;
        right: 20px;
    }

    .pos4{
        top: 150px;
        right: 0;
    }

    .pos5{
        top: 100px;
        right: 0;
    }

</style>
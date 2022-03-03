<template>
    <div id="main">
        <MainJumbotron></MainJumbotron>
      
        <div id="cardContainer">
            <ImgCard v-for="(elemento, index) in imgArrey" :key="index" :send="elemento"></ImgCard>
        </div>

        <WorkingProcessBox></WorkingProcessBox>

        <SendMessageBox></SendMessageBox>
    </div>
</template>

<script>
import MainJumbotron from "./partials/MainJumbotron.vue"
import ImgCard from "./partials/ImgCard.vue"
import WorkingProcessBox from "./partials/WorkingProcessBox.vue"
import SendMessageBox from "./partials/SendMessageBox.vue"


export default {
    name: "MyMain" ,
    components: {
        MainJumbotron,
        ImgCard,
        WorkingProcessBox,
        SendMessageBox
    },

    data() {
        return{
            imgArrey: [
                {src:"../../../public/img/h-2-port-img-2.jpg"},
                {src:"../../../public/img/h-2-port-img-3.jpg"},
                {src:"../../../public/img/h-2-port-img-1.jpg"},
                {src:"../../../public/img/h-2-port-img-4.jpg"},
                {src:"../../../public/img/h-2-port-img-5.jpg"},
                {src:"../../../public/img/h-2-port-img-6.jpg"}
            ]
        }
    }
}
</script>

<style scoped lang="scss">

    #cardContainer{
        display: flex;
        flex-wrap: wrap;
        position: relative;
    }

</style>
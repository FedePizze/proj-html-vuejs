<template>
    <div id="imgCardBox">
        <!-- <img :src="send.src" alt=""> -->
        <img src="../../../public/img/h-2-port-img-1.jpg" alt="">
        <div id="hoverInfo">
            <h3>Illustrations of Novels</h3>
            <h5>Illustration</h5>
        </div>
    </div>
</template>

<script>
export default {
    name: "ImgCard",
    props: {
        send: Object
    },

    created() {
        console.log(this.send)
    }
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #imgCardBox{
        width: calc(100% / 3);
        position: relative;
        margin-top: -4px;

        img{
            width: 100%;
        }

        #hoverInfo{
            position: absolute;
            top: calc(50% - 30px);
            padding: 25px 30px;
            background-color: white;
            z-index: 3;
            display: none;

            h3{
                font-size: 20px;
                font-weight: 500;
            }

            h5{
                padding: 6px 0px;
                font-weight: 500;
                font-style: italic;
            }
        }
        
    }

    #imgCardBox:hover #hoverInfo{
        display: block;
    }
</style>
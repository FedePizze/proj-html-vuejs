<template>
    <a href="#" id="greenButton">
        <img src="../../assets/svg/svg-5.svg" alt="">
    </a>
</template>

<script>
export default {
    name: "ArrowButton"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #greenButton{
        position: absolute;
        width: 40px;
        height: 40px;
        background-color: $Green;
        text-align: center;

        img{
            transform: rotate(-90deg);
            margin-top: 7px;
            width: 65%;
        }
    }

</style>
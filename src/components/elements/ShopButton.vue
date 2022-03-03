<template>
    <a href="#" id="greenButton">
        <img src="../../assets/svg/svg-6.svg" alt="">
    </a>
</template>

<script>
export default {
    name: "ShopButton"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #greenButton{
        position: absolute;
        width: 40px;
        height: 40px;
        background-color: white;
        display: flex;
        justify-content: center;
        align-items: center;

        img{
            width: 60%;
        }
    }

</style>
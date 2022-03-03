<template>
    <a href="#" id="greenButton">
        <img src="../../assets/svg/svg-4.svg" alt="">
    </a>
</template>

<script>
export default {
    name: "CircleButton"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #greenButton{
        position: absolute;
        width: 40px;
        height: 40px;
        background-color: #ee2852;
        display: flex;
        justify-content: center;
        align-items: center;

        img{
            width: 65%;
        }
    }

</style>
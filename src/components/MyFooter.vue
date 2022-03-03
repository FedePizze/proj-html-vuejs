<template>
    <div id="footer">
        <div id="infoBox">
            <div class="box">
                <img src="../../public/img/logo-sidearea-1.png" alt="">
                <h5>Let's Get Creative</h5>
            </div>
            <div class="box">
                <h5>maree.quode@gmail.com</h5>
                <h5>+44645 321 789</h5>
            </div>
            <div class="box">
                <h5>Avenue d'Auderghem 10</h5>
                <h5>1040 Brussels, Belgium</h5>
            </div>
            <div class="box">
                <h5>Stay in touch with us</h5>
                <div id="socialIcon">
                    <a href="#"><i class="fa-brands fa-twitter" style="color: black; width: 13px;"></i></a>
                    <a href="#"><i class="fa-brands fa-pinterest-p" style="color: black; width: 13px;"></i></a>
                    <a href="#"><i class="fa-brands fa-facebook-f" style="color: black; width: 13px;"></i></a>
                    <a href="#"><i class="fa-brands fa-linkedin-in" style="color: black; width: 13px;"></i></a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyFooter"
}
</script>

<style scoped lang="scss">
    @import "../assets/style/colours.scss";

    #footer{
        padding: 60px ;
        background-color: $Green;

        #infoBox{
            width: 65%;
            margin: 0px auto;
            display: flex;
            align-items:flex-start

            img{
                width: 90px;
            }

            .box{
                width: 25%;

                #socialIcon{
                    display: flex;
                    gap: 18.5px;
                    margin-top: 5px;
                }
            }
        }
    }
</style>
<template>
    <div id="jumboBox">
        <div id="jumbotron">
            <div class="jumbo1">
                <div class="direction"><i style="color: white;" class="fa-solid fa-angle-left"></i></div>
            </div>

            <div class="jumbo2">
                <div id="textBox">
                    <h1>Devotion that never <span>ends</span></h1>
                        <h6>Neque porrp quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adpisci velit, sed quia non numquam eius modi</h6>
                        <a href="#" id="button" >READ MORE</a>
                </div>
            </div>

            <div class="jumbo3">
                <img class="imgGuys" src="../../../public/img/h-2-slider-img-15.png" alt="">
                <img class="imgGuys" src="../../../public/img/h-2-slider-img-16.png" alt="">

                <img class="plantImg plant1" src="../../../public/img/h-2-slider-img-12.png" alt="">
                <img class="plantImg plant2" src="../../../public/img/h-2-slider-img-13.png" alt="">
                <img class="plantImg plant3" src="../../../public/img/h-2-slider-img-14.png" alt="">
                <img class="plantImg plant4" src="../../../public/img/h-2-slider-img-17.png" alt="">
                <img class="plantImg plant5" src="../../assets/svg/svg-0.svg" alt="">
                <img class="plantImg plant6" src="../../assets/svg/svg-0.svg" alt="">
            </div>

            <div div class="jumbo1">
                <div div class="direction"><i style="color: white;" class="fa-solid fa-angle-right"></i></div>
            </div>   
        </div>

        <div id="dotLine">
            <div class="dot"></div>
            <div class="dot"></div>
            <div class="dot"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainJumbotron"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #jumbotron{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 30px 0px;

        .jumbo1{
            width: 5%;
            display: flex;
            justify-content: center;
            align-items: center;

            .direction{
                width: 25px;
                height: 25px;
                text-align: center;
                line-height: 25px;
                background-color: $Pink;
                border-radius: 50%;
            }
        }

        .jumbo2{
            width: 45%;

            #textBox{
                width: 60%;
                margin: 0px auto;

                h1{
                    font-size: 60px;
                    font-weight: 300;

                    span{
                        font-size: 70px;
                        font-family: 'Old Standard TT', serif;
                        font-weight: bold;
                    }
                }

                h6{
                    font-size: 12px;
                    font-weight: 400;
                    line-height: 20px;
                    color: grey;
                    margin: 8px 0px 40px 5px;
                }

                #button{
                    border: 3px solid $Pink;
                    padding: 12px 20px;
                    margin-left: 5px;
                    text-decoration: none;
                    font-size: 11px;
                    font-weight: 600;
                    color: black;
                    letter-spacing: 3px;
                }
            }
        }

        .jumbo3{
            width: 45%;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 40px;
            position: relative;

            .imgGuys{
                width: 250px;
            }

            .plantImg{
                position: absolute;
            }

            .plant1{
                width: 35px;
                left:  0;
            }

            .plant2{
                width: 35px;
                left:  30px;
                bottom: 65px;
            }

            .plant3{
                width: 35px;
                right:  150px;
                top: 20px;
            }

            .plant4{
                width: 55px;
                right:  30px;
                bottom: 40px;
            }

            .plant5{
                width: 40px;
                left:  80px;
                top: 20px;
                transform: rotate(-90deg);
            }

            .plant6{
                width: 35px;
                right: 70px;
                top: 90px;
                fill: red;
            }

        }
    }

    #dotLine{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;
        padding: 25px 0px;

        .dot{
            width: 8px;
            height: 8px;
            border-radius: 50%;
            background-color: $Pink;
        }
    }
</style>
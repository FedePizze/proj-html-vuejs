<template>
    <div id="workingProcess">
        <h2>Working<span> process</span></h2>
        <div id="iconBox">
            <div class="elemento">
                <div class="circle"><i class="fa-solid fa-lightbulb" style="font-size: 30px; color:#d8f0e3"></i></div>
                <div class="textIcon">
                    <h4>First theres an idea</h4>
                    <h5>Lorem ipsum dolor sit amet consectetur, adipisicing elit. A saepe itself.</h5>
                </div>
            </div>

            <div class="elemento">
                <div class="circle"><i class="fa-regular fa-comment" style="font-size: 30px; color:#f8d12d"></i></div>
                <div class="textIcon">
                    <h4>Then we talk about</h4>
                    <h5>Lorem ipsum dolor sit amet consectetur, adipisicing elit. A saepe itself.</h5>
                </div>
            </div>

            <div class="elemento">
                <div class="circle"><i class="fa-solid fa-cloud" style="font-size: 30px; color:#80465f"></i></div>
                <div class="textIcon">
                    <h4>And we think about</h4>
                    <h5>Lorem ipsum dolor sit amet consectetur, adipisicing elit. A saepe itself.</h5>
                </div>
            </div>

            <div class="elemento">
                <div class="circle"><i class="fa-solid fa-cloud" style="font-size: 30px; color:#eb6950"></i></div>
                <div class="textIcon">
                    <h4>So we draw along</h4>
                    <h5>Lorem ipsum dolor sit amet consectetur, adipisicing elit. A saepe itself.</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "WorkingProcessBox"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #workingProcess{
        width: 65%;
        margin: 0px auto;
        padding: 50px 0px;
        text-align: center;

        h2{
            font-size: 40px;
            font-weight: 300;
            margin-bottom: 50px;

            span{
                font-size: 45px;
                font-family: 'Old Standard TT', serif;
                font-weight: bold;
            }
        }

        #iconBox{
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-image: url("../../assets/svg/svg-3.svg");
            background-position: top;
            background-size: 85%;
            background-repeat: no-repeat;
            margin: 20px 0px;

            .elemento{
                width: 25%;
                text-align: center;
                display: flex;
                align-items: center;
                flex-direction: column;

                .circle{
                    width: 100px;
                    height: 100px;
                    border-radius: 50%;
                    background-color: $LightBrown;
                    text-align: center;
                    line-height: 100px;
                }

                .textIcon{
                    padding: 20px;

                    h4{
                        font-size: 17px;
                        font-weight: 500;
                        margin-bottom: 10px;
                    }

                    h5{
                        font-size: 10px;
                        font-weight: 500;
                        line-height: 15px;
                        color: gray;
                    }
                }
            }
        }
    }

</style>
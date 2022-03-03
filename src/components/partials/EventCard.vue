<template>
    <div id="cardBox">
        <img src="../../../public/img/h-2-blog-img-1.jpg" alt="">
        <h4>This, way, lover: a detailed guide through new design</h4>
        <h6>By Emily Fields</h6>

        <div id="dateBox">
            <div id="day"><h3>07</h3></div>
            <div id="month"><h5>MAY</h5><h5>'19</h5></div>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f3d0c7" fill-opacity="1" d="M0,0L720,160L1440,0L1440,320L720,320L0,320Z"></path></svg>
        </div>
    </div>
</template>

<script>
export default {
    name: "EventCard."
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #cardBox{
        width: calc(100% / 3);
        padding: 10px;
        position: relative;

        img{
            width: 100%;
            margin-bottom: 15px;
        }

        h6{
            font-size: 12px;
            font-family: 'Old Standard TT', serif;
            margin-top: 15px;
        }

        #dateBox{
            position: absolute;
            top: 0;
            left: 20px;

            #day{
                width: 52.5px;
                height: 40px;
                background-color: $Green;
                text-align: center;
                line-height: 40px;

                h3{
                    font-size: 25px;
                    font-family: 'Cherish', cursive;
                    margin-left: -8px;
                }
            }

            #month{
                width: 52.5px;
                height: 15px;
                padding: 10px 0px;
                background-color: $Pink;
                margin-bottom: -5px;
                text-align: center;
                line-height: 15px;
                display: flex;
                justify-content: center;
                align-items: center;
                gap: 5px;

                h5{
                    color: black;
                    font-weight: 600;
                }
            }
            
            svg{
                transform: rotate(180deg);
            }
        }
    }

</style>
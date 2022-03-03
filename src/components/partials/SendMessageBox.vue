<template>
    <div id="sendMessageBox">
        <div id="sendBox">
            <h2>Want to work with us? Send un<span> a message!</span></h2>
            <h5>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit labore totam optio consectetur, nam, natus aspernatur quam at perferendis ad voluptatibus tempore veritatis, doloremque consequatur culpa voluptatem possimus cum odio.</h5>
            <a id="button">CONTACT</a>
        </div>
    </div>
</template>

<script>
export default {
    name: "SendMessageBox"
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colours.scss";

    #sendMessageBox{
        height: 300px;
        display: flex;
        align-items: center;

        align-items: center;
        background-image: url("../../../public/img/h-2-background-1.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        background-size: 100%;

        #sendBox{
            width: 65%;
            margin: 0px auto;
            text-align: center;

            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;

            h2{
            font-size: 40px;
            font-weight: 300;

                span{
                    font-size: 45px;
                    font-family: 'Old Standard TT', serif;
                    font-weight: bold;
                }
            }

            #button{
                width: 150px;
                background-color: $Green;
                padding: 12px 20px;
                margin-left: 5px;
                text-decoration: none;
                font-size: 11px;
                font-weight: 600;
                color: black;
                letter-spacing: 3px;
                margin-top: 10px;
            }
        }
    }

</style>
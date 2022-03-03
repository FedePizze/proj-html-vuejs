<template>
  <div id="navBar">
    <div class="box">
        <img src="../../public/img/logo-sidearea-1.png" alt="">
    </div>

    <div class="box">
        <nav>
            <ul>
                <li><div class="hover"></div><a href="">HOME</a></li>
                <li><a href="">PAGES</a></li>
                <li><a href="">PORTFOLIO</a></li>
                <li><a href="">BLOG</a></li>
                <li><a href="">SHOP</a></li>
                <li><a href="">ELEMENTS</a></li>
                <li><a href=""><img id="sixDots" src="../assets/svg/svg-1.svg" alt=""></a></li>
            </ul>
        </nav>
    </div>
  </div>
</template>

<script>
export default {
    name: "MyHeader"
}
</script>

<style scoped lang="scss">
    @import "../assets/style/colours.scss";

    #navBar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 95%;
        margin: 20px auto;

        img{
            width: 80%;
        }

        ul{
            display: flex;
            align-items: center;
            gap: 40px;

            li{
                list-style: none;
                position: relative;

                .hover{
                    position: absolute;
                    width: calc(100% + 20px);
                    height: 7px;
                    background-color: $Pink;
                    z-index: -1;
                    left: -10px;
                    bottom: 0;
                }

                a{
                  text-decoration: none;
                  font-size: 11px;
                  font-weight: 600;
                  color: black;
                  letter-spacing: 3px;
                }
            }
        }
    }

</style>
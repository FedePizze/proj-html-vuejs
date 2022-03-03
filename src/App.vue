<template>

  <div>
    <MyHeader></MyHeader>
    <MyMain></MyMain>
    <MyFooter></MyFooter>
  </div>

</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss";
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Old+Standard+TT:ital@1&display=swap');

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
  
</style>

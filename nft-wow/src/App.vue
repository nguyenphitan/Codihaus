<template>
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/>
  <hr>
  <br><br><br><br><br> -->


  <!-- Home -->
  <home/>
  <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

  <!--  -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Home from './view/Home.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Home,
  }
}
</script>

<style scoped>
@import url('./style/main.css');
</style>

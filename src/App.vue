<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <hello></hello>
    <shopcar></shopcar>
  </div>
</template>

<script>
import Hello from './components/Hello';
import shopcar from './components/shop-car';

export default {
  name: 'app',
  components: {
    Hello,shopcar
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

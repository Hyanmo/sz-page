<template>
  <div class="header">@狗老师版权所有</div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="欢迎门外大人"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.header {
  background-color: #f5f5f5;
  padding: 10px;
  text-align: center;
  font-weight: bold;
}
</style>

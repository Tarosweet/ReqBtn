<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <ReqBtn/>
  </div>
</template>

<script>
import ReqBtn from './components/reqBtn.vue'

export default {
  components: { ReqBtn }
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
</style>

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Counter msg="Counter Value" multiply=1></Counter>
    <Counter msg="Counter Value" multiply=5></Counter>
    <Counter msg="Counter Value" multiply=10></Counter>
  </div>
</template>

<script>
import Counter from './components/Counter.vue';

export default {
  name: 'app',
  components: {
    Counter
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

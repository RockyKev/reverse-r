<template>
  <img alt="Vue logo" src="./assets/korn.jpeg">
  <h1> R Я converter</h1>
  <InputConverter />
  <br>


</template>

<script>
import InputConverter from './components/InputConverter.vue'

export default {
  name: 'App',
  components: {
    InputConverter,
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
</style>

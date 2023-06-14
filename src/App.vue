<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');
* {
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}
</style>

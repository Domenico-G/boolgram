<template>
  <div id="app">
    <Nav/>
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Nav from './components/Nav.vue'

export default {
  name: 'App',
  components: {
    Main,
    Nav
 
  }
}
</script>

<style lang="scss">
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: #2c3e50;
}
</style>

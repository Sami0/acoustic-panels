<template>
  <div id="app">
    <img height="540px" width="770px" alt="sound" src="https://images.unsplash.com/photo-1582767916724-808850c4486f?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D">
    
    <panels msg="acoustic panels"/>
  </div>
</template>

<script>
import panels from './components/panels.vue'
export default {
  name: 'App',
  components: {
    panels
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

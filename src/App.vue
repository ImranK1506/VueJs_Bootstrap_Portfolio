<template>
  <div id="app">
    <Navigation/>
    <router-view></router-view>
    <Footer/>
  </div>
</template>

<script>
import Navigation from './components/includes/navigation'
import Footer from './components/includes/footer'

export default {
  name: 'App',
  components: {
    Navigation,
    Footer
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

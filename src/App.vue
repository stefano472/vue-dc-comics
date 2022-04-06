<template>
  <div id="app">
    <Header/>
    <Main/>
    <PanelMenu/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import PanelMenu from './components/PanelMenu.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    PanelMenu,
    Footer
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'DM Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}

.container {
  width: min(80%, 1200px);
  margin: auto;
  padding: 1rem 0;
}
</style>

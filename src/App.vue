<template>
  <div id="app">
    <Header/>
    <Main />
    <PanelMenu/>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import PanelMenu from '@/components/PanelMenu.vue'
import Footer from '@/components/Footer.vue'

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
  @import '@/assets/style/utilities';
</style>

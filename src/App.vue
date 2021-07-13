<template>
  <div id="app">
    <Header/>
    <Main/>
    <SectionBlu/>
    <Footer/>
  </div>
</template>

<script>
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import SectionBlu from './components/SectionBlu.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    SectionBlu,
    Footer,
  }
}
</script>

<style lang="scss">

@import "./style/app.scss"

</style>

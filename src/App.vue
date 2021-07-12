<template>
  <div id="app">
    <Header/>
    <Main/>
    <FooterBlueBar/>
    <FooterMainBar/>
    <FooterBottomBar/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import FooterBlueBar from './components/FooterBlueBar.vue'
import FooterMainBar from './components/FooterMainBar.vue'
import FooterBottomBar from './components/FooterBottomBar.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    FooterBlueBar,
    FooterMainBar,
    FooterBottomBar
  }
}
</script>

<style lang="scss">
@import "./style/app.scss";

body {
  font-family: $roboto;
}
</style>

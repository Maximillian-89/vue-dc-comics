<template>
  <div id="app">
    <Header/>
    <main>
      <Jumbo/>
      <MainTop/>
      <MainBottom/>
    </main>
    <footer>
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainTop from "./components/MainTop.vue";
import MainBottom from "./components/MainBottom.vue";
import Footer from "./components/Footer.vue";
import Jumbo from "./components/Jumbo.vue";

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    MainBottom,
    Footer,
    Jumbo,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common"
</style>

<template>
  <div id="app">
    <Header/>
    <main>
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

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    MainBottom,
    Footer
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common"
</style>

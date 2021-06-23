<template>
  <div id="app">
    <Header />
    <MainTop />
    <MainMiddle />
    <MainBottom />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainTop from './components/MainTop.vue'
import MainMiddle from './components/MainMiddle.vue'
import MainBottom from './components/MainBottom.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    MainMiddle,
    MainBottom,
    Footer
  }
}
</script>

<style>
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import '~@fontsource/oswald/400.css';
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Oswald', sans-serif;
}
</style>

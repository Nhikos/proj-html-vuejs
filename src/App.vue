<template>
  <div id="app">
    <Header />
    <Main />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
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

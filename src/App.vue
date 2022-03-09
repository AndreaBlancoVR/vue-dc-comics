<template>
  <div id="app">
    <HeaderDc />
    <MainDc />
    <FooterDc />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainDc from './components/MainDc.vue'
import FooterDc from './components/FooterDc.vue'

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainDc,
    FooterDc
  }
}
</script>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Greta Sans Condensed Bold","Greta Sans Bold",Arial,sans-serif;
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  
  // max-width: 1280px;
  ul {
    list-style: none;
  }
}
</style>

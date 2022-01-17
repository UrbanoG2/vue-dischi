<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <!-- <Footer></Footer> -->
  </div>
</template>

<script>

import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
// import Footer from "./components/Footer.vue";s

export default {
  name: "App",
  components: {
    Header,
    Main,
    // Footer
  },
};
</script>

<style lang="scss">

  #app {
    height: 100vh;
    background-color: #1E2D3B;
  };

  @import "./assets/scss/style.scss";

  
</style>

<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style>
#app {
  @import url("https://fonts.googleapis.com/css2?family=Titillium+Web:wght@200;300;400;600&display=swap");

  background-image: url("~@/assets/Mobile_Base_Background.png");
  background-position: 0 0;
  background-size: cover;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

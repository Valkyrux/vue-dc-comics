<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Services></Services>
    <FooterTop></FooterTop>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Services from "./components/Services.vue"
import FooterTop from "./components/FooterTop.vue"

export default {
  name: "App",
  components: {
    HelloWorld,
    Header,
    Main,
    Services,
    FooterTop,
  },
};
</script>

<style lang="scss">
#app {
margin: 0;
padding: 0;
box-sizing: border-box;
}
</style>

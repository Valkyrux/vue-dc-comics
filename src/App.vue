<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Services></Services>
    <FooterTop></FooterTop>
    <FooterBottom></FooterBottom>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Services from "./components/Services.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Services,
    FooterTop,
    FooterBottom,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
@import "./assets/scss/partial/_mixins.scss";
</style>

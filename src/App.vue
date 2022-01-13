<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Services></Services>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Services from "./components/Services.vue"

export default {
  name: "App",
  components: {
    HelloWorld,
    Header,
    Main,
    Services,
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

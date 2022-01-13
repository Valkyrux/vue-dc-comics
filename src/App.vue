<template>
  <div id="app">
    <Header></Header>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue"

export default {
  name: "App",
  components: {
    HelloWorld,
    Header,
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

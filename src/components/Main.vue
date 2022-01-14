<template>
  <main>
    <div class="container">
      <div class="main-top">
          --&#62;Content goes Here&#60;--
      </div>
      <ul>
        <Card
        v-for= "(comic, index) in comics"
        :key="index"
        :img-path="comic.thumb"
        :img-descr="comic.type"
        :img-title="comic.series" />
      </ul>
    </div>
  </main>
</template>

<script>
import Card from "./Card.vue";
export default {
  name: "Main",
  components: {
    Card,
  },
  data () {
    return {
      comics: [],
    }
  },
  created() {
    this.comics = require('../assets/dc-comics.json');
  },
};
</script>

<style scoped lang="scss">
  @import "../assets/scss/partial/_mixins.scss";
  @import "../assets/scss/partial/_commons.scss";
  main {
    background-color: black;
  }

  ul {
    @include flex-set(space-between, centre, true);
  }
</style>

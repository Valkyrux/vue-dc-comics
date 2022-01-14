<template>
  <main>
    <div class="">
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
    <button type="button" name="button" @click="console.log(comics)">click</button>
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
    console.log(this.comics);
  },
};
</script>

<style scoped lang="scss">
  main {
    background-color: black;
  }
</style>

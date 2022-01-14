<template>
  <main>
    <div class="">
        --&#62;Content goes Here&#60;--
    </div>
    <ul>
      <Card
        :img-path="ok"
        :img-descr="ciro"
        :img-title= "Ao"
      />
    </ul>

  </main>
</template>

<script>
import Card from "./Card.vue";
export default {
  name: "Main",
  props: {
  },
};
</script>

<style scoped lang="scss">
  main {
    background-color: black;
  }
</style>

<template>
  <li>
    <div class="img-container">
      <img :src="imgPath" :alt="imgDescr">
    </div>
    <h3>{{imgTitle}}</h3>
  </li>
</template>

<script>
export default {
  name: "Card",
  props: ["imgPath", "imgDescr", "imgTitle"],
};
</script>

<style scoped lang="scss">

  li {
    list-style-type: none;
    width: calc(100%/6 - 20px);
  }

  .img-container {
    height: 150px;
    overflow: hidden;
  }

  img {
    width: 100%;
  }

</style>

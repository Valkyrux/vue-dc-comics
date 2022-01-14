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
    color: white;
    margin: calc(50px/6);
  }

  .img-container {
    height: 170px;
    overflow: hidden;
  }

  img {
    width: 100%;
  }

  h3 {
    margin-top: 10px;
    font-size: 0.8em;
    font-weight: normal;
    text-transform: uppercase;
  }

</style>

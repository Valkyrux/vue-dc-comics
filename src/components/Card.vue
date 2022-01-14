<template>
  <li>
    <img :src="imgPath" :alt="imgDescr">
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

</style>

<template>
  <li>
    <a :href="link"><img :src="path">{{text}}</a>
  </li>
</template>

<script>
export default {
  name: "ServiceIcon",
  props: ["link", "path", "text"]
};
</script>

<style scoped lang="scss">
  @import "../assets/scss/partial/_commons.scss";
  @import "../assets/scss/partial/_variables.scss";

  li {
    height: 100%;
  }

  a {
    display: block;
    height: 100%;
    display: flex;
    align-items: center;
    text-transform: uppercase;
    text-decoration: none;
    font-size: 0.8em;
    color: white;
  }

  img {
    height: 40%;
    margin-right: 8px;
  }
</style>

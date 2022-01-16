<template>
  <nav>
    <ul class="container">
      <li>
        <a><img src="./../assets/img/buy-comics-digital-comics.png"> digital comics</a>
      </li>
      <li>
        <a><img src="./../assets/img/buy-comics-digital-comics.png"> digital comics</a>
      </li>
      <li>
        <a><img src="./../assets/img/buy-comics-digital-comics.png"> digital comics</a>
      </li>
      <li>
        <a><img src="./../assets/img/buy-comics-digital-comics.png"> digital comics</a>
      </li>
      <li>
        <a><img src="./../assets/img/buy-comics-digital-comics.png"> digital comics</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Services",
  data() {
    return {
      serviceList: [],
    }
  },
  created() {
    this.serviceList = require('../assets/service-list.json');

  }
};
</script>

<style scoped lang="scss">
  @import "../assets/scss/partial/_commons.scss";
  @import "../assets/scss/partial/_variables.scss";

  nav {
    background-color: $blue;
    color: white;
    height: 100px;
  }

  ul {
    list-style-type: none;
    height: 100%;
    padding: 0;
    display: flex;
    justify-content: space-between;
  }

  li {
    display: flex;
    height: 100%;
  }

  a {
    display: block;
    height: 100%;
    display: flex;
    align-items: center;
  }

  img {
    height: 40%;
  }
</style>

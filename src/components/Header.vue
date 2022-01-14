<template>
  <header>
    <nav class="container">
      <img src="./../assets/img/dc-logo.png" />
      <ul>
        <li>
          <a>menu-item</a>
        </li>
        <li>
          <a>menu-item</a>
        </li>
        <li>
          <a>menu-item</a>
        </li>
        <li>
          <a>menu-item</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/scss/partial/_commons.scss";
@import "../assets/scss/partial/_mixins.scss";

header {
    background-color: #ffffff;
    height: 70px;
}

nav {
  height: 100%;
  @include flex-set(space-between, center);
}

img {
    height: 80%;
}

ul {
    list-style-type: none;
    height: 100%;
    padding: 0;
}

li {
    display: inline-block;
    height: 100%;
    margin: 0 10px;
}

a {
    color: #42b983;
    display: block;
    height: 100%;
    text-transform: uppercase;
    display: flex;
    align-items: center;
    &:active,
    &:hover {
        border-bottom: 2px solid blue;
    }
}
</style>

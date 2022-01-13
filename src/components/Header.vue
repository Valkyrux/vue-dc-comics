<template>
  <header>
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
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
  },
};
</script>

<style scoped lang="scss">
header {
  background-color: #ffffff;
  height: 70px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border: 2px solid white;
}

img {
  height: 80%
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
  display:block;
  height: 100%;
  text-transform: uppercase;
  display:flex;
  align-items: center;
  &:hover,
  &:active {
    border-bottom: 2px solid blue;
  }
}
</style>

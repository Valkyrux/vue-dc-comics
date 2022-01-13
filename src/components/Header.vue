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
}

img {
  height: 80%
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

jCjWhhg8WXg5h5D

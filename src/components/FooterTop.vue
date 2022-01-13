<template>
  <footer>
    <div>
      <h3>Titolo</h3>
      <ul>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
      </ul>
      <h3>Titolo</h3>
      <ul>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
      </ul>
    </div>
    <div>
      <h3>Titolo</h3>
      <ul>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
      </ul>
    </div>
    <div>
      <h3>Titolo</h3>
      <ul>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
        <li><a>a link</a></li>
      </ul>
    </div>
    <img src="./../assets/img/dc-logo-bg.png">
  </footer>
</template>

<script>
export default {
  name: "FooterTop",
  props: {
  },
};
</script>

<style scoped lang="scss">
  footer {
    background-image: url("./../assets/img/footer-bg.jpg");
    display: flex;
    position: relative;
    align-items: flex-start;
    color: white;
    overflow: hidden;
  }

  div {
    margin: 0 10px;
  }

  ul {
    list-style-type: none;
    height: 100%;
    padding: 0;
  }

  img {
    position: absolute;
    right: 0;
    top: 50%;
    transform: translatey(-50%);
  }

</style>

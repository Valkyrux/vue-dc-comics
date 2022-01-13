<template>
  <div class="footer-bottom">
    <button>Sign-Up Now!</button>
    <div class="follow-us">
      <h2>Follow us</h2>
      <ul>
        <li><a><img src="./../assets/img/footer-facebook.png"></a></li>
        <li><a><img src="./../assets/img/footer-facebook.png"></a></li>
        <li><a><img src="./../assets/img/footer-facebook.png"></a></li>
        <li><a><img src="./../assets/img/footer-facebook.png"></a></li>
        <li><a><img src="./../assets/img/footer-facebook.png"></a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBottom",
  props: {
  },
};
</script>

<style scoped lang="scss">
   .footer-bottom{
    background-color: #242526;
    color: white;
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  button {
    background-color: inherit;
    border-radius: 0;
    border: 2px solid blue;
    text-transform: uppercase;
    color: white;
  }

  .follow-us {
    display: flex;
  }

  ul {
    display: flex;
    list-style-type: none;
  }

  li {
    margin: 0 5px;
  }
</style>

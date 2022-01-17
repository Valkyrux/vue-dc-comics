<template>
  <nav>
    <ul class="container">
      <ServiceIcon
        v-for="(service, index) in serviceList"
        :key ="index"
        :link = "service.href"
        :path="require('../assets/img/' + service.imgPath)"
        :text="service.name"/>
    </ul>
  </nav>
</template>

<script>
import ServiceIcon from "./ServiceIcon.vue";
export default {
  name: "Services",
  components: {
    ServiceIcon,
  },
  data() {
    return {
      serviceList: [],
    }
  },
  created() {
    this.serviceList = require('../assets/service-list.json');
  },
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
</style>

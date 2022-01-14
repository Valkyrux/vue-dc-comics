<template>
  <header>
    <nav class="container">
      <img src="./../assets/img/dc-logo.png" />
      <ul>
        <li v-for="(voice,index) in menuVoices" :key="index">
          <a :href="voice.hRef" :class="(index==activeVoice)?'active':''" @click="setActiveVoice(index)">{{voice.title}}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      activeVoice: 1,
      menuVoices: [
        {
          title: "characters",
          hRef: "#"
        },
        {
          title: "comics",
          hRef: "#"
        },
        {
          title: "movies",
          hRef: "#"
        },
        {
          title: "tv",
          hRef: "#"
        },
        {
          title: "games",
          hRef: "#"
        },
        {
          title: "collectibles",
          hRef: "#"
        },
        {
          title: "videos",
          hRef: "#"
        },
        {
          title: "fans",
          hRef: "#"
        },
        {
          title: "news",
          hRef: "#"
        },
        {
          title: "shop",
          hRef: "#"
        },
      ]
    }
  },
  methods: {
    setActiveVoice(index) {
      this.activeVoice = index;
    }
  }
};
</script>

<style scoped lang="scss">
@import "../assets/scss/partial/_commons.scss";
@import "../assets/scss/partial/_mixins.scss";
@import "../assets/scss/partial/_variables.scss";

header {
    background-color: #ffffff;
    height: 70px;
}

nav {
  height: 100%;
  @include flex-set(space-between, center);
}

img {
    height: 66%;
}

ul {
    list-style-type: none;
    height: 100%;
    padding: 0;
}

li {
    display: inline-block;
    height: 100%;
    margin: 0 7px;
}

a {
    color: #000000;
    text-decoration: none;
    display: block;
    font-size: 0.6em;
    height: 100%;
    text-transform: uppercase;
    display: flex;
    align-items: center;
    cursor: pointer;
    &:active,
    &.active,
    &:hover {
        color: $blue;
        border-bottom: 3px solid $blue;
    }
}
</style>

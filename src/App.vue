<template>
  <div id="app">
    <HeaderBool @cards-received="arrMovies = $event" />
    <MainBool :arr-movie-name="arrMovies" />
    <LangFlag />
  </div>
</template>

<script>
import HeaderBool from "./components/HeaderBool.vue";
import MainBool from "./components/MainBool.vue";
import LangFlag from "./main.js";

export default {
  name: "App",
  components: {
    HeaderBool,
    MainBool,
    LangFlag,
  },
  data() {
    return {
      arrMovies: null,
    };
  },
};
</script>

<style lang="scss">
@import "./assets/styles/style.scss";
</style>

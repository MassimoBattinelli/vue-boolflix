<template>
  <div id="app">
    <HeaderBool @cards-received="arrMovies = $event" />
    <MainBool :arr-movie-name="arrMovies" />
  </div>
</template>

<script>
import HeaderBool from "./components/HeaderBool.vue";
import MainBool from "./components/MainBool.vue";

export default {
  name: "App",
  components: {
    HeaderBool,
    MainBool,
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

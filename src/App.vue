<template>
  <div id="app">
    <HeaderBool
      @movie-received="arrMovies = $event"
      @serie-received="arrSeries = $event"
    />
    <MainBool :arr-movie-name="arrMovies" :arr-serie-name="arrSeries" />
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
      arrSeries: null,
    };
  },
};
</script>

<style lang="scss">
@import "./assets/styles/style.scss";
</style>

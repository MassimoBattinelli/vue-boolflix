<template>
  <div id="app">
    <HeaderBool />
  </div>
</template>

<script>
import HeaderBool from "./components/HeaderBool.vue";
export default {
  name: "App",
  components: {
    HeaderBool,
  },
};
</script>

<style lang="scss">
@import "./assets/styles/style.scss";
</style>

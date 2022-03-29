<template>
  <header>
    <h1 class="logo">BOOLFLIX</h1>
    <div class="header-right">
      <label for="movie-search">
        <input
          type="text"
          name="film-search"
          id="film-search"
          placeholder="Digita il titolo"
        />
      </label>
      <button>Cerca</button>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderBoolflix",
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
h1 {
  color: red;
  font-size: 40px;
}
input,
button {
  height: 2.5rem;
  border: none;
}
input {
  padding: 0 1rem;
}
button {
  padding: 0 1rem;
  background: red;
  color: white;
}
</style>

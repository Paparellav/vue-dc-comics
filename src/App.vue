<template>
  <div id="app">
    <AppHeader />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;600;700;800&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: black;
  font-family: "Roboto", sans-serif;
}
</style>

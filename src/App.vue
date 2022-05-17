<template>
  <div id="app">
    <AppHeader />
    <main>-->Content goes here>--</main>
    <section>Qui va la section azzurra</section>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style lang="scss">
$text-color: white;
$blue-color: #0282f9;
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;200;300;400;500;600;700;800&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #1c1c1c;
  font-family: "Roboto", sans-serif;
  color: $text-color;
}

main {
  width: 100%;
  height: 150px;
  display: flex;
  align-items: center;
  padding: 0 4rem;
  font-size: 2rem;
}

section {
  width: 100%;
  height: 130px;
  display: flex;
  align-items: center;
  padding: 0 4rem;
  font-size: 2rem;
  background-color: $blue-color;
}
</style>

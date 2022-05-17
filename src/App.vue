<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppBonus />
    <AppFooter />
    <AppFooterBottom />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppBonus from "./components/AppBonus.vue";
import AppFooter from "./components/AppFooter.vue";
import AppFooterBottom from "./components/AppFooterBottom.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppBonus,
    AppFooter,
    AppFooterBottom,
  },
};
</script>

<style lang="scss">
$text-color: white;
@import url("https://fonts.googleapis.com/css2?family=Signika+Negative:wght@100;200;300;400;500;600;700;800&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #1c1c1c;
  font-family: "Signika Negative", sans-serif;
  color: $text-color;
}
</style>

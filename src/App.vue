<template>
  <div id="app">
    <AppHeader />
    <main>
      <AppMain />
    </main>
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
@import "./style/variables.scss";
@import "./style/common.scss";
</style>

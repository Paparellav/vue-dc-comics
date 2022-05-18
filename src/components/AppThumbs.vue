<template>
  <ul class="thumb">
    <li>
      <img :src="thumbsObj.thumb" alt="thumbsObj.series" />
      <h3>{{ thumbsObj.series }}</h3>
    </li>
  </ul>
</template>

<script>
export default {
  name: "AppThumbs",
  props: ["thumbsObj"],
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";

.thumb {
  width: calc(100% / 6 - 2rem);
  margin: 0 1rem;
  li {
    img {
      width: 180px;
      height: 180px;
      margin-top: 1rem;
    }
    h3 {
      font-size: 1rem;
      font-weight: lighter;
      text-transform: uppercase;
      margin-top: 0.5rem;
    }
  }
}
</style>

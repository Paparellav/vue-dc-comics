<template>
  <div class="thumb">
    <div class="thumb__img">
      <img :src="thumbsObj.thumb" :alt="thumbsObj.series" />
    </div>
    <h3>{{ thumbsObj.series }}</h3>
  </div>
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
  width: calc(100% / 6 - 20px);
  margin: 0 10px;

  &__img {
    margin-top: 1rem;
    width: 160px;
    height: 160px;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top;
    }
  }
  h3 {
    font-size: 0.8rem;
    font-weight: lighter;
    text-transform: uppercase;
    margin-top: 0.5rem;
  }
}
</style>

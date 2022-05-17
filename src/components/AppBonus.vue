<template>
  <div class="bonus-section">
    <div class="bonus__container">
      <ul>
        <li v-for="(item, index) in bonusArray" :key="index">
          <img :src="require(`../assets/img/${item.img}`)" :alt="item.text" />
          <h3>{{ item.text }}</h3>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppBonus",
  data: function () {
    return {
      bonusArray: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC Merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comic Shop Locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$blue-color: #0282f9;

.bonus-section {
  width: 100%;
  background-color: $blue-color;

  .bonus__container {
    width: 60%;
    margin: auto;
    height: 150px;
    display: flex;
    align-items: center;

    ul {
      display: flex;

      li {
        margin-right: 1rem;
        display: flex;
        align-items: center;

        img {
          height: 60px;
        }

        h3 {
          margin: 0 1rem;
          text-transform: uppercase;
          font-size: 1rem;
          font-weight: lighter;
        }
      }
    }
  }
}
</style>

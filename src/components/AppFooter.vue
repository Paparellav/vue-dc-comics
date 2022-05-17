<template>
  <div class="footer-top">
    <div class="footer-top__container">
      <div class="footer-col">
        <h3 class="title">DC Comics</h3>
        <ul>
          <li v-for="(element, index) in primeroArray" :key="index">
            <a href="">{{ element.text }}</a>
          </li>
        </ul>
        <h3 class="title">Shop</h3>
        <ul>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>
      <div class="footer-col">
        <h3 class="title">DC</h3>
        <ul>
          <li v-for="(element, index) in secondArray" :key="index">
            <a href="">{{ element.text }}</a>
          </li>
        </ul>
      </div>
      <div class="footer-col">
        <h3 class="title">Sites</h3>
        <ul>
          <li v-for="(element, index) in thirdArray" :key="index">
            <a href="">{{ element.text }}</a>
          </li>
        </ul>
      </div>
      <div class="footer-col">
        <div>
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooter",
  data: function () {
    return {
      primeroArray: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "Tv",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
      ],
      secondArray: [
        {
          url: "#",
          text: "Terms Of Use",
          active: false,
        },
        {
          url: "#",
          text: "Privacy policy (New)",
          active: true,
        },
        {
          url: "#",
          text: "Ad Choices",
          active: false,
        },
        {
          url: "#",
          text: "Advertising",
          active: false,
        },
        {
          url: "#",
          text: "Jobs",
          active: false,
        },
        {
          url: "#",
          text: "Subscriptions",
          active: false,
        },
        {
          url: "#",
          text: "Talent Workshops",
          active: false,
        },
        {
          url: "#",
          text: "CPSC Cerificates",
          active: false,
        },
        {
          url: "#",
          text: "Ratings",
          active: false,
        },
        {
          url: "#",
          text: "Shop Help",
          active: false,
        },
        {
          url: "#",
          text: "Contact us",
          active: false,
        },
      ],
      thirdArray: [
        {
          url: "#",
          text: "DC",
          active: false,
        },
        {
          url: "#",
          text: "MAD Magazine",
          active: true,
        },
        {
          url: "#",
          text: "DC Kids",
          active: false,
        },
        {
          url: "#",
          text: "DC Universe",
          active: false,
        },
        {
          url: "#",
          text: "DC Power Visa",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$text-color: white;

.footer-top {
  width: 100%;
  height: 380px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;

  .footer-col {
    margin: 0 2rem;
  }

  &__container {
    width: 70%;
    margin: 0 auto;
    display: flex;

    .title {
      padding-top: 1.3rem;
      font-size: 1.3rem;
      text-transform: uppercase;
    }

    ul {
      list-style: none;

      :first-child {
        margin-top: 0.8rem;
      }

      li {
        padding: 0.25rem 0;
        font-size: 0.8rem;

        a {
          text-decoration: none;
          font-weight: 100;
          color: $text-color;
        }
      }
    }

    img {
      width: 100%;
      position: relative;
      bottom: 90px;
      left: 210px;
    }
  }
}
</style>

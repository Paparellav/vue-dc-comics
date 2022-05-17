<template>
  <header class="header">
    <div class="header__container">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul class="header__menu">
          <li
            v-for="(element, index) in menuArray"
            :key="index"
            :class="element.active === true ? 'active' : ''"
          >
            <a href="">{{ element.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      menuArray: [
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
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$text-menu-color: black;
$blue-color: #0282f9;

.header {
  width: 100%;
  background-color: white;

  &__container {
    width: 85%;
    height: 120px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 1.5rem;
  }

  &__logo {
    min-width: 500px;

    img {
      width: 80px;
    }
  }

  &__menu {
    display: flex;
    justify-content: center;

    li {
      margin: 0.4rem;
      padding: 3rem 0.4rem;
      text-transform: uppercase;
      border-bottom: 4px solid transparent;

      &.active {
        border-color: $blue-color;
      }

      &.active a {
        color: $blue-color;
      }

      a {
        color: $text-menu-color;
        text-decoration: none;
        font-weight: 600;
        font-size: 0.9rem;
      }
    }
  }
}

ul {
  list-style: none;
}
</style>

<template>
  <footer class="footer-bottom">
    <div class="footer-bottom__container">
      <div class="sign-up-btn">
        <a href="#">SIGN-UP NOW!</a>
      </div>
      <div class="follow-us-section">
        <h3>FOLLOW US</h3>
        <div class="img-section">
          <img src="../assets/img/footer-facebook.png" alt="footer-facebook" />
          <img src="../assets/img/footer-twitter.png" alt="footer-twitter" />
          <img src="../assets/img/footer-youtube.png" alt="footer-youtube" />
          <img
            src="../assets/img/footer-pinterest.png"
            alt="footer-pinterest"
          />
          <img
            src="../assets/img/footer-periscope.png"
            alt="footer-periscope"
          />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooterBottom",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/variables.scss";

.footer-bottom {
  width: 100%;
  background-color: #303030;

  &__container {
    width: 70%;
    height: 100px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;

    .sign-up-btn {
      min-width: 750px;
      a {
        padding: 0.8rem 1rem;
        text-decoration: none;
        font-size: 1.1rem;
        font-weight: 500;
        border: 2px solid $blue-color;
        background-color: #303030;
        color: $text-color;
      }
    }

    .follow-us-section {
      display: flex;
      align-items: center;
      color: #0a72d4;

      h3 {
        font-size: 1.5rem;
        margin-right: 1rem;
      }

      .img-section img {
        margin: 0 0.8rem;
      }
    }
  }
}
</style>

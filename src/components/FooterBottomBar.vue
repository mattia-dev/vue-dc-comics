<template>
  <div class="social-bar">
    <div class="container">
      <div class="left-content">
        <div class="footer-button">SIGN-UP NOW!</div>
      </div>

      <div class="right-content">
        <div>FOLLOW US</div>

        <ul>
          <li><img src="../assets/footer-facebook.png" alt="fb"></li>
          <li><img src="../assets/footer-twitter.png" alt="tw"></li>
          <li><img src="../assets/footer-youtube.png" alt="yt"></li>
          <li><img src="../assets/footer-pinterest.png" alt="pi"></li>
          <li><img src="../assets/footer-periscope.png" alt="pe"></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'FooterBottomBar',
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

.social-bar {
  height: 100px;
  background-color: $dark-grey;

  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .footer-button {
      color: $white;
      padding: 12px;
      border: 3px solid $light-blue;
      cursor: pointer;
      transition: .2s;

      &:hover {
        background-color: $light-blue;
      }
    }

    .right-content {
      display: flex;
      align-items: center;

      div {
        color: $light-blue;
        font-size: 18px;
        font-weight: 600;
      }

      ul {
        display: flex;
        list-style: none;

        li {
          margin: 0 6px;
          cursor: pointer;

          &:first-child {
            margin-left: 24px;
          }
        }
      }
    }
  }
}
</style>
<template>
  <div class="blue-bar">
    <div class="container">
      <ul>
        <li>
          <a href="#">
            <img src="../assets/buy-comics-digital-comics.png" alt="digital-comics">
            <div>DIGITAL COMICS</div>
          </a>
        </li>

        <li>
          <a href="#">
            <img src="../assets/buy-comics-merchandise.png" alt="merchandise">
            <div>DC MERCHANDISE</div>
          </a>
        </li>

        <li>
          <a href="#">
            <img src="../assets/buy-comics-subscriptions.png" alt="comics subscriptions">
            <div>SUBSCRIPTION</div>
          </a>
        </li>

        <li>
          <a href="#">
            <img src="../assets/buy-comics-shop-locator.png" alt="comics shop locator">
            <div>COMIC SHOP LOCATOR</div>
          </a>
        </li>

        <li>
          <a href="#">
            <img src="../assets/buy-dc-power-visa.svg" alt="dc power visa">
            <div>DC POWER VISA</div>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: 'FooterBlueBar',
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

.blue-bar {
  height: 100px;
  background-color: $light-blue;

  ul {
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    list-style: none;

    li {
      a {
        text-decoration: none;
        display: flex;
        align-items: center;
        color: $white;

        img {
          height: 42px;
          margin-right: 12px;
        }

        div {
          font-size: 14px;
        }
      }
    };
  }
}
</style>
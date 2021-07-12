<template>
  <footer>
    <div class="container">
      <div class="left-content">
        <div class="list-box">
          <ul>
            <li>DC COMICS</li>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Video</li>
            <li>News</li>
          </ul>
          
          <ul>
            <li>SHOP</li>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>

        <div class="list-box">
          <ul>
            <li>DC</li>
            <li>Terms of use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact  us</li>
          </ul>
        </div>

        <div class="list-box">
          <ul>
            <li>SITES</li>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
      </div>

      <div class="right-content"></div>
    </div>
  </footer>
</template>

<script>

export default {
  name: 'FooterMainBar',
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

footer {
  height: 320px;
  background-image: url(../assets/footer-bg.jpg);
  background-size: cover;

  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;

    .left-content {
      flex-grow: .5;
      display: flex;
      justify-content: space-between;
      align-self: center;

      .list-box {
        align-self: flex-start;

        ul {
        list-style: none;

          li {
            color: $grey;
            font-size: 14px;
            margin-bottom: 4px;
            transition: .2s;

            &:not(:first-child) {
              cursor: pointer;
            }

            &:hover:not(:first-child) {
              color: $light-grey;
            }

            &:first-child {
              color: $white;
              font-size: 18px;
              font-weight: 600;
              margin-bottom: 12px;
            }

            &:last-child {
              margin-bottom: 16px;
            }
          }
        }
      }
    }

    .right-content {
      width: 40%;
      background-image: url(../assets/dc-logo-bg.png);
      background-position: center;
      background-size: cover;
    }
  }
}
</style>
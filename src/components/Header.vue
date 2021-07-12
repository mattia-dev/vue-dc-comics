<template>
  <header>
    <div class="container">
      <div class="header-logo">
        <img src="../assets/dc-logo.png" alt="dc-logo">
      </div>

      <nav>
        <ul>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

header {
  height: 80px;
  background-color: $white;

  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
      height: 60px;
      margin: 0 12px;
    }

    nav {
      height: 100%;
    };

    ul {
      list-style: none;
      display: flex;
      font-size: 16px;
      font-weight: 500;
      height: 100%;

      li {
        height: 80px;
        line-height: 70px;
        height: 100%;
        margin: 0 12px;
        padding-top: 5px;
        border-bottom: 5px solid white;
        transition: .2s;

        &:hover {
          color: $light-blue;
          border-bottom: 5px solid $light-blue;
        }
      }
    }
  }
}
</style>
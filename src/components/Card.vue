<template>
  <div class="card-container">
      <img :src="cover" :alt="title">
      <h3>{{title}}</h3>    
      <div>{{price}}</div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    cover: String,
    type: String,
    price: String,
  }
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

.card-container {
    width: calc(100% / 6);
    padding: 12px;
    cursor: pointer;

    &:hover img {
            object-fit: contain;
            opacity: .8;
        }

    img {
        width: 100%;
        height: 176px;
        object-fit: cover;
        object-position: top;
        transition: .2s;
    }

    h3 {
        margin-bottom: 6px;
    }

    div {
        font-size: 14px;
        color: $light-grey;
    }
}
</style>
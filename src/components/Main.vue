<template>
  <main>
    <div class="container">
      <Card
        v-for="(comic, index) in comics"
        :key="index"
        :title="comic.series"
        :cover="comic.thumb"
        :type="comic.type"
        :price="comic.price"
      />
    </div>
  </main>
</template>

<script>
import Card from './Card.vue';

export default {
  name: 'Main',
  components: {
    Card,
  },
  props: {
    comics: Array,
  }
}
</script>

<style lang="scss" scoped>
@import "../style/colors.scss";

main {
    background-color: $black;
    color: $white;
    
    .container {
      display: flex;
      flex-wrap: wrap;
      padding: 12px 0;
    }
}
</style>
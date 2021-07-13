<template>
  <main>
    <Card
      v-for="(element, index) in comics"
      :key="index"
      :thumb="element.thumb"
      :price="element.price"
      :title="element.series"
      :type="element.type"
    />
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
  },
  created() {
    console.log(this.comics);
  },
};
</script>

<style scoped lang="scss">
@import '../style/colors';

main {
  background-color: black;
  height: 80px;
  color: $text-white;
  z-index: 1;
}
</style>

<template>
  <div class="product-card">
    <img :src="thumb" />
    <h3>{{ title }}</h3>
    <h4>{{ price }}</h4>
    <h4>{{ type }}</h4>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    thumb: String,
    price: String,
    title: String,
    type: String,
  },
};
</script>

<style scoped lang="scss">
@import '../style/colors';
</style>

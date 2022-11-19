<template>
  <div class="product">
    <a href="#">
      <img :src="img" class="product__image" :alt="title" />
    </a>
    <h4 class="product__title">{{ title }}</h4>
    <span class="product__price">£{{ price }}</span>
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  img: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  price: {
    type: Number,
    required: true,
  },
});
</script>

<style lang="scss" scoped></style>

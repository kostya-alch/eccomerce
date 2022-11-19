<template>
  <div class="about-brand">
    <h3 class="about-brand__title">What makes our brand different</h3>
    <div class="about-brand-blocks">
      <div class="about-brand-block" v-for="(block, index) of aboutBrands" :key="index">
        <img :src="block.img" :alt="block.title" class="about-brand-block__image" />
        <h4 class="about-brand-block__title">{{ block.title }}</h4>
        <span class="about-brand-block__body">{{ block.body }}</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const aboutBrands = [
  {
    img: "/icons/delivery.svg",
    title: "Next day as standard",
    body: "Order before 3pm and get your order the next day as standard",
  },
  {
    img: "/icons/checkmark.svg",
    title: "Made by true artisans",
    body: "Handmade crafted goods made with real passion and craftmanship",
  },
  {
    img: "/icons/purchase.svg",
    title: "Unbeatable prices",
    body: "For our materials and quality you won’t find better prices anywhere",
  },
  {
    img: "/icons/sproit.svg",
    title: "Recycled packaging",
    body: "We use 100% recycled to ensure our footprint is more manageable",
  },
];
</script>

<style scoped lang="scss">
.about-brand {
  padding: 80px 80px 130px 80px;

  &__title {
    text-align: center;
    font-size: 24px;
    color: #2a254b;
    margin: 0 0 84px 0;
    font-weight: 400;
  }

  &-blocks {
    display: grid;
    grid-template-columns: repeat(4, 210px);
    justify-content: space-between;
    color: #2a254b;
  }

  &-block {
    &__image {
      display: block;
      margin-bottom: 12px;
    }

    &__title {
      margin: 0 0 12px 0;
      font-size: 20px;
    }

    &__body {
      font-size: 16px;
      line-height: 1.5;
    }
  }
}
</style>

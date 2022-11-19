<template>
  <div class="products-container">
    <div class="products">
      <ProductItem
        v-for="product of products"
        :key="product.id"
        :img="product.img"
        :price="product.price"
        :title="product.title"
      />
    </div>
    <a href="#" class="products-link">View collection</a>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import ProductItem from "@/components/ProductItem.vue";

const products = ref([
  {
    id: 1,
    img: "/img/products/product1.jpg",
    title: "The Dandy chair",
    price: 250,
  },
  {
    id: 2,
    img: "/img/products/product2.jpg",
    title: "Rustic Vase Set",
    price: 155,
  },
  {
    id: 3,
    img: "/img/products/product3.jpg",
    title: "The Silky Vase",
    price: 125,
  },
  {
    id: 4,
    img: "/img/products/product4.jpg",
    title: "The Lucy Lamp",
    price: 399,
  },
]);
</script>

<style lang="scss" scoped>
.products {
  display: flex;
  grid-template-columns: repeat(4, 1fr);
  column-gap: 20px;
  padding: 0 80px;
  margin-bottom: 64px;

  &-container {
    margin-bottom: 56px;
  }

  &-link {
    display: block;
    text-align: center;
    color: #2a254b;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
}
</style>

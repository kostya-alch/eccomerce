<template>
  <div class="container">
    <Header />
    <Hero />
    <AboutBrand />
    <products />
  </div>
</template>

<script setup>
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import AboutBrand from "@/components/AboutBrand.vue";
import Products from "@/components/Products.vue";
</script>

<style lang="scss">
@font-face {
  font-family: "Satoshi";
  src: local("Satoshi"), url("@/assets/fonts/Satoshi-Regular.woff2") format("woff2");
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Clash Display";
  src: local("Clash Display"), url("@/assets/fonts/ClashDisplay-Medium.woff2") format("woff2");
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "Clash Display";
  src: local("Clash Display"), url("@/assets/fonts/ClashDisplay-Regular.woff2") format("woff2");
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Satoshi", sans-serif;
  font-size: 16px;
}

img {
  max-width: 100%;
}

.container {
  max-width: 1140px;
  margin: auto;
}
</style>

<template>
  <div class="hero">
    <div class="hero-info">
      <div class="hero-info-text">
        <h2 class="hero-info__title">
          Luxury homeware for people who love timeless design quality
        </h2>
        <span class="hero-info__body">Shop the new Spring 2022 collection today</span>
      </div>
      <a href="#" class="hero-info__link">View Collection</a>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.hero {
  background: url("/img/hero.jpg");
  height: 704px;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding-right: 80px;

  &-info {
    max-width: 630px;
    height: 444px;
    background: #fff;
    padding: 50px 55px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    &__title {
      font-size: 32px;
      line-height: 1.5;
      color: #22202e;
      font-weight: 400;
      margin: 0 0 20px 0;
    }

    &__body {
      font-size: 18px;
      line-height: 150%;
      color: #5b5676;
      font-weight: 400;
    }

    &__link {
      text-decoration: none;
      color: #2a254b;

      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>

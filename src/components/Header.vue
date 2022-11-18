<template>
  <header class="header">
    <div class="header-top">
      <div class="header-top-search">
        <img src="/icons/search.svg" alt="search" />
      </div>
      <a href="#" class="header-logo">Avion</a>
      <div class="header-top-right">
        <div class="header-top-right__cart">
          <a href="#"> <img src="/icons/cart.svg" alt="cart" /></a>
        </div>
        <div class="header-top-right__user">
          <a href="#"> <img src="/icons/user-avatar.svg" alt="user" /></a>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
.header {
  height: 132px;
  background: #fff;

  &-top {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    height: 70px;

    &-right {
      display: flex;
      align-items: center;

      &__cart {
        margin-right: 16px;
      }
    }
  }

  &-logo {
    color: #22202e;
    font-size: 24px;
    line-height: 30px;
    font-weight: 400;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
}
</style>

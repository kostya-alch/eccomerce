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
    <div class="header-menu">
      <a
        :href="element.path"
        v-for="(element, index) of menu"
        :key="index"
        class="header-menu__link"
      >
        {{ element.name }}</a
      >
    </div>
  </header>
</template>

<script setup lang="ts">
const menu = [
  {
    name: "Plant pots",
    path: "/plant",
  },
  {
    name: "Ceramics",
    path: "/ceramics",
  },
  {
    name: "Tables",
    path: "/tables",
  },

  {
    name: "Plant pots",
    path: "/plant",
  },
  {
    name: "Chairs",
    path: "/chairs",
  },
  {
    name: "Crockery",
    path: "/crockery",
  },
  {
    name: "Tableware",
    path: "/tableware",
  },
  {
    name: "Cutlery",
    path: "/cutlery",
  },
];
</script>

<style lang="scss">
.header {
  height: 132px;
  background: #fff;

  &-top {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    height: 70px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    margin: 0 28px;

    &-right {
      display: flex;
      align-items: center;
      justify-content: flex-end;

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
    text-align: center;

    &:hover {
      text-decoration: underline;
    }
  }

  &-menu {
    height: 62px;
    display: flex;
    justify-content: center;
    align-items: center;

    &__link {
      margin: 0 22px;
      text-decoration: none;
      color: #726e8d;
      line-height: 22px;
      font-style: normal;

      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>

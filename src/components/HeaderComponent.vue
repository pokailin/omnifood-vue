<template>
  <header class="header" :class="{ 'nav-open': openNav }">
    <a href="#">
      <img class="logo" src="../assets/omnifood-logo.png" alt="Logo" width="1212" height="63" />
    </a>
    <nav class="main-nav">
      <ul class="main-nav-list">
        <li><a class="main-nav-link" href="#how">How It Works</a></li>
        <li><a class="main-nav-link" href="#meals">Meals</a></li>
        <li><a class="main-nav-link" href="#testimonials">Testimonials</a></li>
        <li><a class="main-nav-link" href="#pricing">Pricing</a></li>
        <li><a class="main-nav-link nav-cta" href="#cta">Try for free</a></li>
      </ul>
    </nav>

    <button class="btn-mobile-nav">
      <ion-icon class="icon-mobile-nav" name="menu-outline" @click="openNav = !openNav"></ion-icon>
      <ion-icon
        class="icon-mobile-nav"
        name="close-outline"
        @click="openNav = !openNav"
        v-if="openNav"
      ></ion-icon>
    </button>
  </header>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core';

export default defineComponent({
  name: 'HeaderView',
  setup() {
    let openNav = false;
    // const navLink = ref(null);

    // onMounted(() => {
    //   console.log(navLink.value);
    // });

    return { openNav };
  },
});
</script>

<style>
.header {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #fdf2e9;

  /* Because we want header to be sticky later */
  height: 9.6rem;
  padding: 0 4.8rem;
}

.logo {
  height: 2.2rem;
  width: auto;
}

.main-nav-list {
  display: flex;
  list-style: none;
  align-items: center;
  gap: 4.8rem;
}

.main-nav-link:link,
.main-nav-link:visited {
  display: inline-block;
  text-decoration: none;
  color: #333;
  font-weight: 500;
  font-size: 1.8rem;
  transition: color 300ms;
}

.main-nav-link:hover,
.main-nav-link:active {
  color: #cf711f;
}

.main-nav-link.nav-cta:link,
.main-nav-link.nav-cta:visited {
  background-color: #e67e22;
  padding: 1.2rem 2.4rem;
  border-radius: 9px;
  color: #fff;
}

.main-nav-link.nav-cta:hover,
.main-nav-link.nav-cta:active {
  background-color: #cf711f;
}

/* MOBILE MENU */
.btn-mobile-nav {
  border: none;
  background: none;
  cursor: pointer;
  display: none;
}

.icon-mobile-nav {
  font-size: 4.8rem;
}

.icon-mobile-nav[aria-label='close outline'] {
  display: none;
}
</style>

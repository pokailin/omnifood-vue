<template>
  <header class="header" :class="{ 'nav-open': openNav, 'sticky-navigation': isStickyNavigation }">
    <a href="#">
      <img class="logo" src="../assets/omnifood-logo.png" alt="Logo" width="1212" height="63" />
    </a>
    <nav class="main-nav">
      <ul class="main-nav-list">
        <li v-for="navLink in navLinks" :key="navLink.href">
          <a
            class="main-nav-link"
            :class="{ 'nav-cta': navLink.href === 'cta' }"
            :href="`#${navLink.href}`"
            @click="handleClick"
          >
            {{ navLink.name }}
          </a>
        </li>
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
import { defineComponent, ref } from 'vue';
import links from '../data/headerNavLinks';

export default defineComponent({
  name: 'HeaderView',
  props: {
    isStickyNavigation: {
      required: true,
      type: Boolean,
    },
  },
  setup() {
    const openNav = ref(false);
    const navLinks = links;

    const handleClick = () => {
      if (openNav.value) {
        openNav.value = !openNav.value;
      }
    };

    return { openNav, navLinks, handleClick };
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

.sticky-navigation {
  z-index: 999;
  position: fixed;
  top: 0;
  bottom: 0;
  height: 8rem;
  width: 100%;
  padding-block: 0;
  background-color: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(25px);
  box-shadow: 0 1.2rem 3.2rem rgba(0, 0, 0, 0.03);
}
</style>

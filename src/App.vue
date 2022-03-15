<template>
  <HeaderComponent />
  <main>
    <Hero />
    <FeaturedComponent />
    <HowItWorks />
    <MealsComponent />
    <TestimonialsComponent />
    <PricingComponent />
    <CallToAction />
  </main>
  <FooterView />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HeaderComponent from './components/HeaderComponent.vue';
import Hero from './components/Hero.vue';
import HowItWorks from './components/HowItWorks.vue';
import FeaturedComponent from './components/FeaturedComponent.vue';
import MealsComponent from './components/MealsComponent.vue';
import TestimonialsComponent from './components/TestimonialsComponent.vue';
import PricingComponent from './components/PricingComponent.vue';
import CallToAction from './components/CallToAction.vue';
import FooterView from './components/FooterView.vue';

@Options({
  components: {
    HeaderComponent,
    Hero,
    FeaturedComponent,
    HowItWorks,
    MealsComponent,
    TestimonialsComponent,
    PricingComponent,
    CallToAction,
    FooterView,
  },
})
export default class App extends Vue {}
</script>

<style>
@import url('./assets/style.css');
@import url('./assets/queries.css');

#app {
  font-family: 'Rubik', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #555;
  line-height: 1;
  font-weight: 400;
}
</style>

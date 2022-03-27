<template>
  <section class="section-featured">
    <div class="container">
      <h2 class="heading-featured-in">As featured in</h2>
      <div class="logos">
        <img
          v-for="(logo, index) in featuredLogos"
          :key="index"
          :src="require(`../assets/logos/${logo.src}`)"
          :alt="logo.alt"
          :width="logo.width"
          :height="logo.height"
        />
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import logos from '@/data/featuredLogos';

export default defineComponent({
  name: 'FeaturedComponent',
  setup() {
    const featuredLogos = logos;

    return { featuredLogos };
  },
});
</script>

<style>
.section-featured {
  padding: 4.8rem 0 3.2rem 0;
}

.heading-featured-in {
  font-size: 1.4rem;
  text-transform: uppercase;
  letter-spacing: 0.75px;
  font-weight: 500;
  text-align: center;
  margin-bottom: 2.4rem;
  color: #888;
}

.logos {
  display: flex;
  justify-content: space-around;
}

.logos img {
  height: 3.2rem;
  width: auto;
  filter: brightness(0);
  opacity: 50%;
}
</style>

<template>
  <section class="section-hero">
    <div class="hero">
      <div class="hero-text-box">
        <h1 class="heading-primary">A healthy meal delivered to your door, every single day</h1>
        <p class="hero-description">
          The smart 365-days-per-year food subscription that will make you eat healthy again. Tailored to
          your personal tastes and nutritional needs.
        </p>
        <a href="#cta" class="btn btn--full margin-right-sm">Start eating well</a>
        <a href="#how" class="btn btn--outline">Learn more &darr;</a>
        <div class="delivered-meals">
          <div class="delivered-imgs">
            <img
              v-for="index in 6"
              :key="index"
              :src="require('../assets/customers/customer-' + index + '.jpg')"
              alt="Customer photo"
              width="128"
              height="128"
            />
          </div>
          <p class="delivered-text"><span>250,000+</span> meals delivered last year!</p>
        </div>
      </div>
      <div class="hero-img-box">
        <picture>
          <source srcset="../assets/hero-min.webp" type="image/webp" />
          <source srcset="../assets/hero-min.png" type="image/png" />
          <img
            class="hero-img"
            src="../assets/hero-min.png"
            alt="Woman enjoying food, meals in storage container, and food bowls on a table"
            width="1200px"
            height="1184px"
          />
        </picture>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  components: {},
})
export default class Hero extends Vue {}
</script>

<style>
.section-hero {
  background: #fdf2e9;
  padding: 4.8rem 6.4rem 9.6rem;
}

.hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 9.6rem;
  max-width: 130rem;
  margin: 0 auto;
  align-items: center;
}

.hero-description {
  font-size: 2rem;
  line-height: 1.6;
  margin-bottom: 4.8rem;
}

.btn--full:link,
.btn--full:visited {
  background-color: #e67e22;
  color: #fff;
}

.btn--full:hover,
.btn--full:active {
  background-color: #cf771f;
}

.btn--outline:link,
.btn--outline:visited {
  background-color: #fff;
  box-shadow: inset 0 0 0 2px #e67e22;
  color: #e67e22;
}

.btn--outline:hover,
.btn--outline:active {
  background-color: #fdf2e9;
  box-shadow: inset 0 0 0 2px #e67e22;
  color: #e67e22;
}

.hero-img {
  width: 100%;
  height: 100%;
}

.delivered-meals {
  display: flex;
  align-items: center;
  gap: 1.6rem;
  margin-top: 8rem;
}

.delivered-imgs {
  display: flex;
}

.delivered-imgs img {
  height: 4.8rem;
  width: 4.8rem;
  border-radius: 50%;
  border: 2px solid #fdf2e9;
}

.delivered-imgs img:not(:last-child) {
  margin-right: -1.6rem;
}

.delivered-text {
  font-size: 1.8rem;
  font-weight: 600;
}

.delivered-text span {
  color: #cf711f;
  font-weight: 700;
}
</style>

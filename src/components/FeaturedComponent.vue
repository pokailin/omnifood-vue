<template>
  <section class="section-featured">
    <div class="container">
      <h2 class="heading-featured-in">As featured in</h2>
      <div class="logos">
        <img src="../assets/logos/techcrunch.png" alt="Techcrunch logo" />
        <img src="../assets/logos/business-insider.png" alt="Business Insider logo" />
        <img src="../assets/logos/the-new-york-times.png" alt="The New York Times logo" />
        <img src="../assets/logos/forbes.png" alt="Forbes logo" />
        <img src="../assets/logos/usa-today.png" alt="USA Today logo" />
      </div>
    </div>
  </section>
</template>

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
  filter: brightness(0);
  opacity: 50%;
}
</style>

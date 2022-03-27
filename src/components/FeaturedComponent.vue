<template>
  <section class="section-featured">
    <div class="container">
      <h2 class="heading-featured-in">As featured in</h2>
      <div class="logos">
        <img src="../assets/logos/techcrunch.png" alt="Techcrunch logo" width="562" height="80" />
        <img
          src="../assets/logos/business-insider.png"
          alt="Business Insider logo"
          width="252"
          height="80"
        />
        <img
          src="../assets/logos/the-new-york-times.png"
          alt="The New York Times logo"
          width="609"
          height="80"
        />
        <img src="../assets/logos/forbes.png" alt="Forbes logo" width="306" height="80" />
        <img src="../assets/logos/usa-today.png" alt="USA Today logo" width="428" height="80" />
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
  width: auto;
  filter: brightness(0);
  opacity: 50%;
}
</style>

<template>
  <section class="section-testimonials" id="testimonials">
    <div class="testimonials-container">
      <span class="subheading">Testimonials</span>
      <h2 class="heading-secondary">Once you try it, you can't go back</h2>
      <div class="testimonials">
        <figure class="testimonial">
          <img
            class="testimonial-img"
            src="../assets/customers/dave.jpg"
            alt="Photo of customer Dave Bryson"
          />
          <blockquote class="testimonial-text">
            Inexpensive, healthy and great-tasting meals, without even having to order manually! It feels
            truly magical.
          </blockquote>
          <cite class="testimonial-name">&mdash; Dave Bryson</cite>
        </figure>
        <figure class="testimonial">
          <img
            class="testimonial-img"
            src="../assets/customers/ben.jpg"
            alt="Photo of customer Ben Hadley"
          />
          <blockquote class="testimonial-text">
            The AI algorithm is crazy good, it chooses the right meals for me every time. It's amazing
            not to worry about food anymore!
          </blockquote>
          <cite class="testimonial-name">&mdash; Ben Hadley</cite>
        </figure>
        <figure class="testimonial">
          <img
            class="testimonial-img"
            src="../assets/customers/steve.jpg"
            alt="Photo of customer Steve Miller"
          />
          <blockquote class="testimonial-text">
            Omnifood is a life-saver! I just started a company, so there's no time for cooking. I
            couldn't live without my daily meals now!
          </blockquote>
          <cite class="testimonial-name">&mdash; Steve Miller</cite>
        </figure>
        <figure class="testimonial">
          <img
            class="testimonial-img"
            src="../assets/customers/hannah.jpg"
            alt="Photo of customer Hannah Smith"
          />
          <blockquote class="testimonial-text">
            I got Omnifood for the whole family, and it frees up so much time! Plus, everything is
            organic and vegan and without plastic.
          </blockquote>
          <cite class="testimonial-name">&mdash; Hannah Smith</cite>
        </figure>
      </div>
    </div>
    <div class="gallery">
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-1.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
        <!-- CAN ONLY USE INSIDE OF FIGURE -->
        <!-- <figcaption>Caption</figcaption> -->
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-2.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-3.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-4.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-5.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-6.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-7.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-8.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-9.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-10.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-11.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="../assets/gallery/gallery-12.jpg"
          alt="Photo of beautifully arranged food"
          width="800"
          height="800"
        />
      </figure>
    </div>
  </section>
</template>

<style>
.section-testimonials {
  background-color: #fdf2e9;
  display: grid;
  grid-template-columns: 55fr 45fr;
  align-items: center;
}

.testimonials-container {
  padding: 9.6rem;
}

.testimonials {
  display: grid;
  grid-template-columns: 1fr 1fr;
  row-gap: 4.8rem;
  column-gap: 8rem;
}

.testimonial-img {
  width: 6.4rem;
  height: 6.4rem;
  border-radius: 50%;
  margin-bottom: 1.2rem;
}

.testimonial-text {
  font-size: 1.8rem;
  line-height: 1.8;
  margin-bottom: 1.6rem;
}

.testimonial-name {
  font-size: 1.6rem;
  color: #6f6f6f;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.6rem;
  padding: 1.6rem 1.6rem 1.6rem 0;
}

.gallery-item {
  overflow: hidden;
}

.gallery-item img {
  display: block;
  width: 100%;
  height: auto;
  transition: transform 400ms;
}

.gallery-item img:hover {
  transform: scale(1.1);
}
</style>

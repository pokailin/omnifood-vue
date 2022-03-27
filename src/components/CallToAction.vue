<template>
  <section class="cta-section" id="cta">
    <div class="container">
      <div class="cta">
        <div class="cta-text-box">
          <h2 class="heading-secondary">Get your first meal for free!</h2>
          <p class="cta-text">
            Healthy, tasty and hassle-free meals are waiting for you. Start eating well today. You can
            cancel or pause anytime. And the first meal is on us.
          </p>

          <form class="cta-form" action="#">
            <div>
              <label for="full-name">Full Name</label>
              <input id="full-name" type="text" placeholder="John Smith" required />
            </div>
            <div>
              <label for="email">Email Address</label>
              <input id="email" type="email" placeholder="me@example.com" required />
            </div>

            <div>
              <label for="select-where">Where did you hear from us?</label>
              <select name="" id="select-where" required>
                <option value="">Please choose one option:</option>
                <option value="friends">Friends and family</option>
                <option value="youtube">Youtube video</option>
                <option value="podcast">Podcast</option>
                <option value="facebook">Facebook ad</option>
                <option value="other">Other</option>
              </select>
            </div>

            <button class="btn btn--form" type="submit">Sign up now</button>
          </form>
        </div>
        <div class="cta-img-box" role="img" aria-label="Woman enjoying food"></div>
      </div>
    </div>
  </section>
</template>

<style>
.cta-section {
  padding: 4.8rem 0 12.8rem;
}

.cta {
  overflow: hidden;
  background-image: linear-gradient(to right bottom, #eb984e, #e67e22);
  box-shadow: 0 2.4rem 4.8rem rgba(0, 0, 0, 0.15);
  display: grid;
  grid-template-columns: 2fr 1fr;
  border-radius: 11px;
}

.cta .heading-secondary {
  /* color: #45260a; */
  color: inherit;
  margin-bottom: 3.2rem;
}

.cta-text-box {
  padding: 4.8rem 6.4rem 6.4rem 6.4rem;
  color: #45260a;
}

.cta-text {
  font-size: 1.8rem;
  line-height: 1.8;
  margin-bottom: 4.8rem;
}

.cta-img-box {
  background-image: linear-gradient(to right bottom, rgba(235, 151, 78, 0.35), rgba(230, 125, 34, 0.35)),
    url('../assets/eating.jpg');
  background-size: cover;
  background-position: center;
  /* border-top-right-radius: 11px;
  border-bottom-right-radius: 11px; */
}

.cta-form {
  display: grid;
  grid-template-columns: 1fr 1fr;
  column-gap: 3.2rem;
  row-gap: 2.4rem;
}

.cta-form label {
  display: block;
  font-size: 1.6rem;
  font-weight: 500;
  margin-bottom: 1.2rem;
}

.cta-form input,
.cta-form select {
  width: 100%;
  padding: 1.2rem;
  font-size: 1.8rem;
  font-family: inherit;
  color: inherit;
  border: none;
  background-color: #fdf2e9;
  border-radius: 9px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}

.cta-form input::placeholder {
  color: #aaa;
}

.cta *:focus {
  outline: none;
  box-shadow: 0 0 0 0.8rem rgba(253, 242, 233, 0.5);
}
</style>

<template>
  <section class="pricing-section" id="pricing">
    <div class="container">
      <span class="subheading">Pricing</span>
      <h2 class="heading-secondary">Eating well without breaking the bank</h2>
    </div>

    <div class="container grid grid--2-cols margin-bottom-md">
      <div class="pricing-plan">
        <header class="plan-header">
          <p class="plan-name">Starter</p>
          <p class="plan-price"><span>$</span>399</p>
          <p class="plan-text">per month. That's just $13 per meal!</p>
        </header>
        <ul class="list">
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>1 meal per day</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>Order from 11am to 9pm</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>Delivery is free</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="close-outline"></ion-icon>
            <span>Delivery is free</span>
          </li>
        </ul>
        <div class="plan-sign-up">
          <a href="#" class="btn btn--full">Start eating well</a>
        </div>
      </div>
      <div class="pricing-plan pricing-plan--complete">
        <header class="plan-header">
          <p class="plan-name">Complete</p>
          <p class="plan-price"><span>$</span>649</p>
          <p class="plan-text">per month. That's just $11 per meal!</p>
        </header>
        <ul class="list">
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span><strong>2</strong> meals per day</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>Order 24/7</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>Delivery is free</span>
          </li>
          <li class="list-item">
            <ion-icon class="list-icon" name="checkmark-outline"></ion-icon>
            <span>Get access to latest recipes</span>
          </li>
        </ul>
        <div class="plan-sign-up">
          <a href="#" class="btn btn--full">Start eating well</a>
        </div>
      </div>
    </div>

    <div class="container grid">
      <aside class="plan-details">
        Prices include all applicable taxes. You can cancel at any time. Both plans also include the
        following:
      </aside>
    </div>

    <div class="container grid grid--4-cols">
      <div class="feature">
        <ion-icon class="feature-icon" name="infinite-outline"></ion-icon>
        <p class="feature-title">Never cook again!</p>
        <p class="feature-text">
          Our subscriptions cover 365 days per year, even including major holidays.
        </p>
      </div>
      <div class="feature">
        <ion-icon class="feature-icon" name="nutrition-outline"></ion-icon>
        <p class="feature-title">Local and organic</p>
        <p class="feature-text">
          Our cooks only use local, fresh, and organic products to prepare your meals.
        </p>
      </div>
      <div class="feature">
        <ion-icon class="feature-icon" name="leaf-outline"></ion-icon>
        <p class="feature-title">No waste</p>
        <p class="feature-text">
          All our partners only use reusable containers to package all your meals.
        </p>
      </div>
      <div class="feature">
        <ion-icon class="feature-icon" name="pause-outline"></ion-icon>
        <p class="feature-title">Pause anytime</p>
        <p class="feature-text">
          Going on vacation? Just pause your subscription, and we refund unused days.
        </p>
      </div>
    </div>
  </section>
</template>

<style>
.pricing-section {
  padding: 9.6rem 0;
}

.pricing-plan {
  border-radius: 11px;
  padding: 4.8rem;
  width: 75%;
}

.pricing-plan:first-child {
  justify-self: end;
  box-shadow: inset 0 0 0 5px #fdf2e9;
}

.pricing-plan--complete {
  background-color: #fdf2e9;
  position: relative;
  overflow: hidden;
}

.pricing-plan--complete::after {
  background-color: #ffd43b;
  color: #333;
  content: 'Best Value';
  position: absolute;
  top: 7%;
  right: -15%;
  transform: rotate(45deg);
  text-transform: uppercase;
  font-size: 1.4rem;
  font-weight: 700;
  padding: 0.8rem 6.4rem;
}

.plan-header {
  text-align: center;
  margin-bottom: 4.8rem;
}

.plan-name {
  color: #cf711f;
  font-weight: 600;
  font-size: 2rem;
  text-transform: uppercase;
  letter-spacing: 0.75px;
  margin-bottom: 3.2rem;
}

.plan-price {
  font-size: 6.2rem;
  font-weight: 600;
  color: #333;
  margin-bottom: 1.6rem;
}

.plan-price span {
  font-size: 3rem;
  font-weight: 500;
  margin-right: 0.8rem;
}

.plan-text {
  font-size: 1.6rem;
  line-height: 1.6;
  color: #6f6f6f;
}

.plan-sign-up {
  text-align: center;
  margin-top: 4.8rem;
}

.plan-details {
  font-size: 1.6rem;
  line-height: 1.6;
  text-align: center;
}

.feature-icon {
  background-color: #fdf2e9;
  border-radius: 50%;
  padding: 1.6rem;
  color: #e67e22;
  font-size: 3.2rem;
  margin-bottom: 3.2rem;
}

.feature-title {
  font-size: 2.4rem;
  color: #333;
  font-weight: 700;
  margin-bottom: 1.6rem;
}

.feature-text {
  font-size: 1.8rem;
  line-height: 1.8;
}
</style>

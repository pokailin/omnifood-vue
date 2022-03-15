<template>
  <footer class="footer">
    <div class="container grid grid--footer">
      <div class="logo-col">
        <a href="#" class="footer-logo">
          <img class="logo" src="../assets/omnifood-logo.png" alt="Logo" />
        </a>
        <ul class="social-links">
          <li>
            <a class="footer-link" href="#">
              <ion-icon class="social-icon" name="logo-instagram"></ion-icon>
            </a>
          </li>
          <li>
            <a class="footer-link" href="#">
              <ion-icon class="social-icon" name="logo-facebook"></ion-icon>
            </a>
          </li>
          <li>
            <a class="footer-link" href="#">
              <ion-icon class="social-icon" name="logo-twitter"></ion-icon>
            </a>
          </li>
        </ul>
        <p class="copyright">Copyright &copy; 2027 by Omnifood, Inc. All rights reserved.</p>
      </div>
      <div class="address-col">
        <p class="footer-heading">Contact us</p>
        <address class="contacts">
          <p>623 Harrison St., 2nd floor, San Francisco, CA 94107</p>
          <p>
            <a class="footer-link" href="tel:415-201-6370">415-201-6370</a><br />
            <a class="footer-link" href="mailto:hello@omnifood.com">hello@omnifood.com</a>
          </p>
        </address>
      </div>
      <nav class="nav-col">
        <p class="footer-heading">Accounts</p>
        <ul class="footer-nav">
          <li>
            <a class="footer-link" href="#">Create account</a>
          </li>
          <li>
            <a class="footer-link" href="#">Sign in</a>
          </li>
          <li>
            <a class="footer-link" href="#">iOS app</a>
          </li>
          <li>
            <a class="footer-link" href="#">Android app</a>
          </li>
        </ul>
      </nav>
      <nav class="nav-col">
        <p class="footer-heading">Company</p>
        <ul class="footer-nav">
          <li>
            <a class="footer-link" href="#">About Omnifood</a>
          </li>
          <li>
            <a class="footer-link" href="#">For business</a>
          </li>
          <li>
            <a class="footer-link" href="#">Cooking partners</a>
          </li>
          <li>
            <a class="footer-link" href="#">Careers</a>
          </li>
        </ul>
      </nav>
      <nav class="nav-col">
        <p class="footer-heading">Resources</p>
        <ul class="footer-nav">
          <li>
            <a class="footer-link" href="#">Recipe Directory</a>
          </li>
          <li>
            <a class="footer-link" href="#">Help center</a>
          </li>
          <li>
            <a class="footer-link" href="#">Privacy & Terms</a>
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<style>
.footer {
  padding: 12.8rem 0;
  border-top: 1px solid #eee;
  /* background-color: #eee; */
}

.grid--footer {
  grid-template-columns: 1.5fr 1.5fr 1fr 1fr 1fr;
}

.logo-col {
  display: flex;
  flex-direction: column;
}

.footer-logo {
  display: block;
  margin-bottom: 3.2rem;
}

.social-links {
  display: flex;
  gap: 2.4rem;
  list-style: none;
}

.social-icon {
  font-size: 2.4rem;
}

.copyright {
  font-size: 1.4rem;
  line-height: 1.6;
  color: #767676;
  margin-top: auto;
}

.footer-heading {
  font-size: 1.8rem;
  font-weight: 500;
  margin-bottom: 4rem;
}

.contacts {
  font-style: normal;
  font-size: 1.6rem;
  line-height: 1.6;
}

.contacts p:first-child {
  margin-bottom: 2.4rem;
}

.footer-nav {
  display: flex;
  flex-direction: column;
  gap: 2.4rem;
  list-style: none;
}

.footer-link:link,
.footer-link:visited {
  text-decoration: none;
  font-size: 1.6rem;
  color: #767676;
  transition: color 300ms;
}

.footer-link:hover,
.footer-link:active {
  color: #555;
}
</style>

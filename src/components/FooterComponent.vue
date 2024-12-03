<script setup>
</script>

<template>
  <footer>
    <div class="footer__container">
      <div class="footer__column">
        <h1>DudeShape</h1>
        <p class="footer__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed eiusmod tempor incididunt ut labore at dolore.</p>
        <div class="footer__socials">
          <h2>Follow Us :</h2>
        </div>
        <div class="footer__social">
          <a href="#" class="footer__social-link">
            <img src="@/assets/img/Group%208872.png" alt="">
          </a>
          <a href="#" class="footer__social-link">
            <img src="@/assets/img/Group%208872.png" alt="">
          </a>
          <a href="#" class="footer__social-link">
            <img src="@/assets/img/Group%208872.png" alt="">
          </a>
          <a href="#" class="footer__social-link">
            <img src="@/assets/img/Group%208872.png" alt="">
          </a>
        </div>
      </div>

      <div class="footer__column">
        <h3 class="footer__title">Take a tour</h3>
        <ul class="footer__links">
          <li><a href="#" class="footer__link">Features</a></li>
          <li><a href="#" class="footer__link">Pricing</a></li>
          <li><a href="#" class="footer__link">Product</a></li>
          <li><a href="#" class="footer__link">Support</a></li>
        </ul>
      </div>

      <div class="footer__column">
        <h3 class="footer__title">Our company</h3>
        <ul class="footer__links">
          <li><a href="#" class="footer__link">About Us</a></li>
          <li><a href="#" class="footer__link">Blog</a></li>
          <li><a href="#" class="footer__link">Media</a></li>
          <li><a href="#" class="footer__link">Contact Us</a></li>
        </ul>
      </div>
      <div class="footer__column">
        <h3 class="footer__title">Subscribe</h3>
        <p class="footer__text">Subscribe to get the latest <br> news from us</p>
        <input type="email" class="footer__input" placeholder="Enter adreess" />
        <img class="input__img" src="@/assets/img/Frame%2054.png" alt="">
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  background-color: #305F64;
  color: white;
  padding: 40px 20px;
}

.footer__container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 30px;
  max-width: 1200px;
  margin: 0 auto;
}

.footer__column {
  display: flex;
  flex-direction: column;
  gap: 16px;
}
.footer__socials h2 {
  font-size: 20px;
  font-family: "Montserrat", sans-serif;
}
.footer__socials {
  display: flex;
}

.footer__text {
  margin-bottom: 15px;
}
.footer__title h3 {
  font-weight: 700;
  font-family: "Montserrat", sans-serif;
}
.footer__social {
  display: flex;
  gap: 15px;
}
.footer__column a {
  display: flex;
  gap: 16px;
  font-size: 18px;
  font-family: "DM Sans", sans-serif;
}
.footer__socials {
  display: flex;
  gap: 15px;
}

.footer__social-link {
  color: white;
  text-decoration: none;
  font-size: 16px;
}

.footer__social-link:hover {
  color: #FFB624;
}

.footer__title {
  font-weight: 700;
  margin-bottom: 10px;
}

.footer__links {
  list-style: none;
  padding: 0;
}
.footer__column h1 {
  font-size: 24px;
}
.footer__link {
  color: white;
  text-decoration: none;
  font-size: 16px;
  margin-bottom: 8px;
}

.footer__link:hover {
  color: #FFB624;
}

.footer__input {
  padding: 10px;
  font-size: 16px;
  border-radius: 10px;
  border: none;
  margin-top: 10px;
  width: 100%;

}
.input__img{
  position: relative;
  top: -50px;
  right: -260px;
  height: 28px;
  width: 28px;
}
</style>
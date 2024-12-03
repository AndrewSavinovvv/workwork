<script setup>

</script>

<template>
    <div class="hero ">
      <div class="hero__main">
        <div class="hero__main-left">
            <h1 class="hero__main-title">
              We Help You <br> Make Modern Furniture
            </h1>
            <p class="hero__main-text">We will help you to make an elegant <br> and luxurious interior designed <br> by professional interior designer.</p>
        </div>
        <div class="hero__main-right">
          <img src="@/assets/img/poster.png" alt="">
        </div>
      </div>
      <div class="hero__main-mobile">
        <div class="hero__main-mobile-first">
          <h1>We Help You Make <br> Modern Furniture</h1>
          <p>All of our furniture uses the best materials and <br> choices for our customers.All of our furniture <br> uses the best materials </p>
          <button class="hero__btn">Explore More</button>
          <div class="hero__main-mobile-second">
            <img src="@/assets/img/poster2.png" alt="">
          </div>
        </div>
      </div>
    </div>
</template>

<style scoped>
.hero__main {
  display: flex;
  align-items: center;
  position: relative;
}
.hero__main-left {
  background: #154444;
  width: 620px;
  height: 469px;
  z-index: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 120px;
  position: relative;
  margin-right: -140px;
}
.hero__main-title {
  font-size: 56px;
  font-weight: 700;
  font-family: "Montserrat", sans-serif;
  color: white;
  margin-bottom: 30px;
}
.hero__main-text {
  color: white;
  font-family: "DM Sans", sans-serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 29px;
}
.hero__main-right {
  position: relative;
  z-index: 0;
}
.hero__main-mobile {
  display: none;
}
@media (max-width: 777px) {
  .hero__main {
    display: none;
  }
  .hero__main-mobile {
    display: flex;
    flex-direction: column;
    background: #154444;
    padding-top: 49px;
    padding-left: 24px;
    padding-right: 24px;
  }
  .hero__main-mobile-first{
    color: white;
  }
  .hero__btn {
    border: none;
    padding: 10px 32px;
    color: #154444;
    font-size: 14px;
    font-family: "DM Sans", sans-serif;
    margin-bottom: 40px;
  }
  .hero__main-mobile-first p {
    margin-bottom: 30px;
  }
  .hero__main-mobile-first h1 {
    margin-bottom: 12px;
  }
  .hero__main-mobile-second{
    display: flex;
    justify-content: center;
  }
}
@media (max-width: 1236px) {
 .hero__main-title {
   font-size: 30px;
 }
  .hero__main-right{
    overflow: hidden;
  }
}
</style>
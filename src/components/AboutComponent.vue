<script setup>
import img from "@/assets/icon/shield.svg"

const aboutItems = [
  {
    img: img ,
    title: "Best Quality",
    text: "All of our furniture uses the best materials and choices",
  },
  {
    img: img ,
    title: "Free Shpping",
    text: "All of our furniture uses the best materials and choices",
  },
  {
    img: img ,
    title: "Free Shpping",
    text: "All of our furniture uses the best materials and choices",
  },
];
</script>

<template>
  <div class="about container">
    <div class="about__left">
      <h2>About Us</h2>
      <p>All of our furniture uses the best materials and choices for our customers.</p>
      <div v-for="(item, index) in aboutItems" :key="index" class="about__item">
        <img :src="item.img" alt="About" />
        <div class="about__item-text">
          <h4>{{ item.title }}</h4>
          <p>{{ item.text }}</p>
        </div>
      </div>
    </div>
    <div class="about__right">
      <div class="about__image-wrapper">
        <img src="@/assets/img/poster3.png" alt="About image" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.about {
  display: flex;
  padding-top: 140px;
  gap: 116px;
}
.about__item {
  display: flex;
  align-items: flex-start;
  gap: 23px;
}
.about__left h2 {
  color: #244D4D;
  font-size: 32px;
  font-weight: 700;
  font-family: "Montserrat", sans-serif;
  margin-bottom: 20px;
}
.about__left p {
  color: #383738;
  font-size: 20px;
  font-family: "DM Sans", sans-serif;
  margin-bottom: 40px;
}
.about__item-text h4 {
  color: #244D4D;
  font-size: 20px;
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
}
.about__item-text p {
  color: #383738;
  font-size: 18px;
  font-family: "DM Sans", sans-serif;
  margin-top: 15px;
}
@media (max-width: 890px) {
  .about {
    display: flex;
    flex-direction: column;
  }
  .about__left h2 {
    font-size: 24px;
    font-weight: 600;
    padding-left: 24px;
  }
  .about__left p {
    font-size: 12px;
    padding-left: 24px;
    margin-bottom: 30px;
  }
  .about__item-text h4{
    font-size: 14px;
    font-weight: 600;

  }
  .about__item-text p {
    font-size: 10px;
    margin-top: 4px;
    padding-left: 0 !important;
  }
  .about__item img {
    width: 28px;
    height: 28px;
    padding-left: 24px;
  }
  .about__item {
    gap: 18px;
  }
  .about__right {
    display: flex;
    justify-content: center;
    position: relative;
  }
  .about__image-wrapper {
    position: relative;
    display: inline-block;
  }
  .about__image-wrapper::after {
    content: "";
    position: absolute;
    background: #DEE4E2;
    height: 348px;
    width: 370px;
    top: 10px;
    left: 0px;
    z-index: 0;
  }
  .about__image-wrapper img {
    position: relative;
    z-index: 1;
    width: 350px;
    height: 341px;
  }
}
</style>
<script setup>
import img from "@/assets/icon/furn.svg"

const furnitureItems = [
  { imgSrc: img, title: "Living Room" },
  { imgSrc: img, title: "Bedroom" },
  { imgSrc: img, title: "Kitchen" },
  { imgSrc: img, title: "Dining Room" },
  { imgSrc: img, title: "Office" },
  { imgSrc: img, title: "Hallway" }
];
</script>

<template>
  <div class="furniture container">
    <h1>All Furniture</h1>
    <nav class="furniture__nav">
      <ul class="furniture__nav-list">
        <li>Shop By Room</li>
        <li>Shop By Category</li>
        <li>Shop By Style</li>
      </ul>
    </nav>
    <div class="furniture__main">
      <div class="furniture__main-left">
        <div class="furniture__main-left-img">
          <img src="@/assets/img/fur.png" alt="">
        </div>
      </div>
      <div class="furniture__main-right">
        <div v-for="(item, index) in furnitureItems" :key="index" class="furniture__main-right-block">
          <img :src="item.imgSrc" alt="Furniture Icon">
          <h4>{{ item.title }}</h4>
        </div>
      </div>
    </div>
    <div class="furniture__hero">
      <div class="furniture__hero-left">
        <div class="furniture__hero-left-img">
          <img src="@/assets/img/fur-hero.png" alt="">
        </div>
      </div>
      <div class="furniture__hero-right">
        <h1>Our customers are verry <br> importan to us</h1>
        <p>All of our furniture uses the best matials and choices for our customers.All of our furniture uses the best materials and choices for our customers.</p>
        <div class="furniture__hero-right-user">
          <img src="@/assets/img/Ellipse%2028.png" alt="">
          <div class="user__name">
            <span>Mh Jibon</span>
            <div class="user__footer">
              <img src="@/assets/img/star%202.png" alt="">
              <span>4.8</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.furniture {
  padding-top: 140px;
}
.furniture h1 {
  color: #244D4D;
  font-size: 32px;
  font-weight: 700;
  font-family: "Montserrat", sans-serif;
  margin-bottom: 30px;
  text-align: center;
}
.furniture__nav-list{
  display: flex;
  justify-content: center;
  gap: 100px;
}
.furniture__nav-list li {
  color: #919090;
  font-size: 24px;
  font-weight: 400;
  font-family: "DM Sans", sans-serif;
  position: relative;
  cursor: pointer;
}
.furniture__nav-list li::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 40px;
  width: 0;
  height: 2px;
  background: #154444;
  transition: width 0.3s ease;
}
.furniture__nav-list li:hover {
  color: #244d4d;
  font-weight: 400;
}
.furniture__nav-list li:hover::after {
  width: 50%;
}
.furniture__main {
  margin-top: 99px;
  display: flex;
  gap: 103px;
}
.furniture__main-left-img {
  position: relative;
  z-index: 1;
}
.furniture__main-left-img:after {
  content: "";
  position: absolute;
  background: #154444;
  height: 389px;
  width: 552px;
  top: -30px;
  left: -30px;
  z-index: -1;
}
.furniture__main-right {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: space-between;
}
.furniture__main-right-block {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  color: #808080;
  font-size: 16px;
  font-family: "DM Sans", sans-serif;
  font-weight: 500;
  width: 222px;
  height: 90px;
  border: 1px solid #D9DCE5;
  transition:  0.3s ease-in-out, background 0.3s ease-in-out;
}
.furniture__main-right-block h4 {
  margin-top: 16px;
}
.furniture__main-right-block:hover {
  color: white;
  background: #154444;
}
.furniture__main-right-block img:hover {
  fill: white;
}
.furniture__hero {
  padding-top: 140px;
  display: flex;
  align-items: center;
  gap: 80px;
}
.furniture__hero-left-img {
  position: relative;
}
.furniture__hero-left-img:after {
  content: "";
  position: absolute;
  background: #154444;
  height: 492px;
  width: 492px;
  top: 0px;
  left: -100px;
  z-index: -1;
  border-radius: 50%;
}
.furniture__hero-right {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.furniture__hero-right h1 {
  text-align: start;
}
.furniture__hero-right p {
  color: #383738;
  font-size: 20px;
  font-family: "DM Sans", sans-serif;
  margin-bottom: 30px;
}
.furniture__hero-right-user{
  display: flex;
  gap: 10px;
  align-items: center;
}
.user__name{
  color: black;
  font-family: "DM Sans", sans-serif;
  font-weight: 500;
  font-size: 16px;
}

</style>
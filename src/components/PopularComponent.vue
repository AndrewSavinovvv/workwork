<script setup>
import CardComponent from "@/components/СardComponent.vue";
import cardImage from "@/assets/img/card.png";
import cardIcon1 from "@/assets/icon/card-icon2.svg";
import cardIcon2 from "@/assets/icon/card-icon.svg";

const cards = [
  {
    imgSrc: cardImage,
    title: "White Swan Chair",
    price: "40$",
    icons: [cardIcon1, cardIcon2],
  },
  {
    imgSrc: cardImage,
    title: "White Swan Chair",
    price: "40$",
    icons: [cardIcon1, cardIcon2],
  },
  {
    imgSrc: cardImage,
    title: "White Swan Chair",
    price: "40$",
    icons: [cardIcon1, cardIcon2],
  },
];
</script>

<template>
  <div class="popular container">
    <div>
      <h1>Our Popular Furniture</h1>
      <div class="popular__text">
        <p>
          All of our furniture uses the best materials and choices for our
          customers. All of our furniture uses the best materials and choices
          for our customers.
        </p>
        <div class="popular__text-arrow">
          <div class="popular__text-arrow-item">
            <img src="@/assets/icon/arrow-left.svg" alt="Arrow Left" />
          </div>
          <div class="popular__text-arrow-item">
            <img src="@/assets/icon/arrow-right.svg" alt="Arrow Right" />
          </div>
        </div>
      </div>
    </div>
    <div class="popular__block">
      <button class="popular__block-btn">More</button>
    </div>
    <div class="popular__cards">
      <CardComponent
          v-for="(card, index) in cards"
          :key="index"
          :imgSrc="card.imgSrc"
          :title="card.title"
          :price="card.price"
          :icons="card.icons"
      />
    </div>
  </div>
</template>

<style scoped>
.popular {
  padding-top: 140px;
}
.popular__text {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.popular h1 {
  color: #244D4D;
  font-size: 32px;
  font-weight: 700;
  font-family: "Montserrat", sans-serif;
}
.popular__text p {
  margin-top: 20px;
  color: #383738;
  font-size: 20px;
  font-family: "DM Sans", sans-serif;
}
.popular__text-arrow{
  display: flex;
  gap: 10px;
}
.popular__text-arrow img {
  width: 14px;
  height: 14px;
}
.popular__text-arrow-item{
  display: flex;
  align-items: center;
  justify-content: center;
  background: #ECF4FF;
  width: 40px;
  height: 40px;
  border-radius: 50px;
  cursor: pointer;
}
.popular__block-btn{
  color: #FF5F00;
  font-size: 20px;
  font-family: "DM Sans", sans-serif;
  border: none;
  background: none;
}
.popular__block{
  display: flex;
  justify-content: end;
}
.popular__cards {
  display: flex;
  gap: 30px;
  margin-top: 13px;
}
@media (max-width: 777px) {
  .popular ,.popular__cards{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .popular__text-arrow{
    display: none;
  }
  .popular__text p {
    padding-left: 12px;
  }
}
</style>
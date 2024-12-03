<script setup>
defineProps({
  imgSrc: String,
  title: String,
  price: String,
  icons: Array,
});
</script>

<template>
  <div class="card">
    <img :src="imgSrc" alt="Card Image" class="card__image" />
    <div class="card__header">
      <h2 class="card__title">{{ title }}</h2>
      <div class="card__icons">
        <img v-for="(icon, index) in icons" :key="index" :src="icon" alt="Icon" class="card__icon" />
      </div>
    </div>
    <div class="card__footer">
      <span class="card__price">{{ price }}</span>
      <button class="card__button">Buy Now</button>
    </div>
  </div>
</template>

<style scoped>
.card {
  background: white;
  width: 380px;
  height: 380px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  overflow: hidden;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}
.card__image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.card__header {
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card__title {
  color: #244d4d;
  font-size: 20px;
  font-weight: 500;
  font-family: "DM Sans", sans-serif;
}
.card__icons {
  display: flex;
  gap: 8px;
}
.card__icon {
  width: 24px;
  height: 24px;
}
.card__footer {
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card__price {
  color: #154444;
  font-family: "DM Sans", sans-serif;
  font-size: 24px;
  font-weight: 500;
}
.card__button {
  background: #244d4d;
  border: none;
  border-radius: 6px;
  color: white;
  padding: 8px 16px;
  font-family: "DM Sans", sans-serif;
  font-size: 14px;
  cursor: pointer;
}
</style>
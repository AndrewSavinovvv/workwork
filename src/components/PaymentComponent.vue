<script setup>
import photo from "@/assets/img/pay.png"

const pay = [
  { img: photo },
  { img: photo },
  { img: photo },
  { img: photo },
  { img: photo },
]
</script>

<template>
  <div class="payment container">
    <h2 class="payment__title">Trusted by 20,000+ companies</h2>
    <div class="payment__list">
      <div v-for="(item, index) in pay" :key="index" class="payment__item">
        <img :src="item.img" alt="logo" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.payment__title {
  color: #154444;
  text-align: center;
  font-size: 32px;
  font-family: "DM Sans", sans-serif;
}
.payment {
  padding-top: 120px
}
.payment__list{
  display: flex;
  justify-content: space-between;
  margin-top: 49px;
}
@media (max-width: 777px) {
  .payment {
    width: 100%;
  }
  .payment__item img{
    width: 57px;
    height: 20px;
  }
  .payment__list {
    padding: 5px;
    margin-top: 26px;
  }
  .payment__title {
    font-size: 18px;
  }
}
</style>
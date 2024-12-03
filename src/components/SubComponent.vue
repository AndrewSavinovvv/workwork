<script setup>
</script>

<template>
  <div class="sub container">
    <h2>
      Subscribe to get the latest news <br> about us
    </h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed <br> eiusmod tempor incididunt ut labore at dolore.</p>
    <div class="sub__input-wrapper">
      <input class="sub__input" type="text" placeholder="Enter your email">
      <button class="sub__button">Register</button>
    </div>
  </div>
</template>

<style scoped>
.sub {
  margin-top: 140px;
  color: white;
  text-align: center;
  background: #305F64;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 140px;
  padding-bottom: 53px;
}

.sub h2 {
  padding-top: 62px;
  font-size: 32px;
  font-weight: 700;
  font-family: Montserrat;
}

.sub__input-wrapper {
  position: relative;
  width: 471px;
  margin-top: 50px;
}

.sub__input {
  width: 100%;
  height: 67px;
  border-radius: 10px;
  border: none;
  padding: 0 20px 0 50px;
  font-size: 16px;
  box-sizing: border-box;
  background-color: white;
  background-image: url('@/assets/icon/Group 16.svg');
  background-repeat: no-repeat;
  background-position: 15px center;
  background-size: 16px;
}

.sub__input::before {
  content: "url";
  position: absolute;
  left: 15px;
  top: 50%;
  transform: translateY(-50%);
  color: white;
  font-size: 22px;
}

.sub__button {
  position: absolute;
  right: 21px;
  top: 10px;
  height: 52px;
  padding: 0 20px;
  background-color: #FFB624;
  color: white;
  border: none;
  border-radius: 10px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  font-family: "DM Sans", sans-serif;
}

.sub__button:hover {
  background-color: #1b6c69;
}

.sub p {
  margin-top: 20px;
  font-size: 20px;
}
</style>
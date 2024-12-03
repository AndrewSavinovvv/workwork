<script setup>

</script>

<template>
 <header class="header container">
   <div class="header__logo">DudeShape</div>
   <nav class="header__nav">
     <ul class="header__nav__list">
       <li>Home</li>
       <li>About</li>
       <li>Features</li>
       <li>Contact</li>
     </ul>
   </nav>
   <div class="header__icon">
    <div>
      <img src="@/assets/icon/search.svg" alt="">
    </div>
     <div>
       <img src="@/assets/icon/burger.svg" alt="">
     </div>
   </div>
   <div class="burger__menu">
     <span></span>
     <span></span>
     <span></span>
   </div>
 </header>
</template>

<style scoped>
.header__nav__list {
  font-family: "DM Sans", sans-serif;
  color: #161616;
  list-style: none;
  font-size: 16px;
  font-weight: 400;
  display: flex;
}
.header__nav__list {
  display: flex;
  gap: 50px;
}
.header__logo {
  font-family: "Montserrat", sans-serif;
  color: #244D4D;
  font-size: 24px;
  font-weight: 700;
}
header {
  display: flex;
  justify-content: space-between;
  padding: 47px 0 34px 0;
}
.header__icon {
  display: flex;
  gap: 38px;
}
.burger__menu {
  display: none;
  flex-direction: column;
  justify-content: space-between;
  width: 31px;
  height: 18px;
  cursor: pointer;
}
.burger__menu span {
  display: block;
  width: 100%;
  height: 4px;
  background-color: #244D4D;
  border-radius: 2px;
}
@media (max-width: 777px) {
  .header__nav__list {
    display: none;
  }
  header {
    padding-top: 40px;
    padding-bottom: 40px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between !important;
  }
  .burger__menu {
    display: flex;
    padding-right: 24px;
  }
  .header__icon {
    display: none;
  }
  .header__logo{
    padding-left: 24px;
  }
}
@media (max-width: 1236px) {
  header {
    justify-content: center;
  }
  .header__nav__list {
    display: none;
  }
  .header__icon {
    display: none;
  }
}
</style>
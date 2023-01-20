<template>
  <div class="container">
    <div class="header">
      <img src="../assets/svg/fake-logo.svg" class="header__img" alt="fake" />

      <div class="nav">
        <a href="#" class="nav__link">Форум</a>
        <a href="#" class="nav__link">Новые товары</a>
        <a href="#" class="nav__link">Вопросы по закупкам</a>
      </div>

      <input type="search" class="header__search" placeholder="Поиск товаров" />

      <div class="header-buttons">
        <a href="#" class="nav-button">
          <img src="../assets/svg/orders.svg" class="nav-button__img" alt="" />
          <p class="nav-button__tittle">Заказы</p>
        </a>

        <a href="#" class="nav-button">
          <img src="../assets/svg/login.svg" class="nav-button__img" alt="" />
          <p class="nav-button__tittle">Войти</p>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  width: 1320px;
}

.nav__link:hover {
  color: #d7576d;
}

.nav-button__tittle:hover {
  color: #d7576d;
}

.header {
  margin: 0 auto;
  width: 1320px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  padding-top: 30px;
  padding-bottom: 30px;
}

.header__img {
  width: 81px;
}

.nav {
  width: 468px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.nav__link {
  margin: 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;

  color: #323232;
  text-decoration: none;
}

.header__search {
  padding: 0;

  width: 320px;
  height: 40px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;

  text-align: center;
  border-radius: 20px;
  border: solid 0;

  background-color: #fdf9f9;
  color: #323232;
}

.header-buttons {
  width: 127px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.nav-button {
  width: 43px;
  height: 48px;

  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  text-decoration: none;
}

.nav-button__img {
  width: 30px;
}

.nav-button__tittle {
  margin: 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 14px;

  color: #323232;
}
</style>
<template>
  <div class="footer">
    <a href="#" class="footer__link">Форум</a>
    <a href="#" class="footer__link">Новые товары</a>
    <a href="#" class="footer__link">Вопросы по закупкам</a>
    <a href="#" class="footer__link">Поиск товаров</a>
    <a href="#" class="footer__link">Заказы</a>
    <a href="#" class="footer__link">Войти</a>
  </div>
</template>

<style>
.footer {
  margin: 0 auto;
  width: 625px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  padding-top: 46px;
  padding-bottom: 46px;
}

.footer__link {
  margin: 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  text-decoration-line: underline;

  color: #323232;
}

.footer__link:hover {
  color: #d7576d;
}
</style>
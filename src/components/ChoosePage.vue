<template>
  <div class="pages">
    <p class="pages__title">Страница:</p>
    <div class="page">
      <button class="page__button">«</button>
      <input class="page__input" type="text" placeholder="1" />
      <button class="page__button">»</button>
    </div>
  </div>
</template>

<style>
.pages {
  margin: 0 auto;
  width: 130px;
  height: 71px;

  display: flex;
  flex-direction: column;
  justify-content: space-between;

  padding-top: 34px;
  padding-bottom: 34px;
}

.pages__title {
  margin: 0 auto;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;

  color: #323232;
}

.page {
  margin: 0;
  width: 130px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.page__button {
  margin: 0;
  width: 30px;
  height: 30px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;

  /* display: flex;
    justify-content: center;
    align-items: center; */

  border-radius: 2px;
  border: solid #eedfe0 1px;
  background-color: #ffffff;
  color: #323232;
}

.page__button:hover {
  border: solid #d7576d 1px;
}

.page__input {
  margin: 0;
  width: 28px;
  height: 28px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  text-align: center;

  padding: 0;

  border-radius: 2px;
  border: solid #eedfe0 1px;
  background-color: #ffffff;
  color: #323232;
}
</style>
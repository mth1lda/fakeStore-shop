<template>
  <div class="good-card">
    <div class="card-cont">
      <div class="img-container">
        <img src="../assets/good.jpg" class="good-card__img" alt="" />
      </div>

      <!-- <div class="stars">
        <img src="../assets/svg/star.svg" class="stars__star" alt="" />
        <img src="../assets/svg/star.svg" class="stars__star" alt="" />
        <img src="../assets/svg/star.svg" class="stars__star" alt="" />
        <img src="../assets/svg/star.svg" class="stars__star" alt="" />
        <img src="../assets/svg/star.svg" class="stars__star" alt="" />
      </div> -->

      <star-raiting></star-raiting>
    </div>
    <div class="good-info">
      <h1 class="good-info__name">Название товара</h1>
      <div class="price">
        <h2 class="price__tittle">Цена</h2>
        <p class="price__price">$</p>
      </div>

      <div>
        <p class="good-info__info">
          Плащ из искусственной кожи<br />

          - Длинный двубортный плащ с поясом из искусственной кожи<br />
          - Застёжка на пуговицах<br />
          - Рукава-регланы<br />
          - 2 внешних кармана<br />
          - По низу рукава регулируемая пата<br />
          - Длина: 123,6 см
        </p>
      </div>

      <div class="card-buttons">
        <button class="card-buttons__button">Заказать</button>
        <button class="card-buttons__button">Подробнее</button>
      </div>
    </div>
  </div>
</template>

<script>
import StarRaiting from "../components/StarRaiting.vue";

export default {
  name: "GoodCard",
  components: {
    StarRaiting,
  },
};
</script>


<style>
.good-card {
  width: 625px;
  height: 329px;

  padding-top: 20px;
  padding-left: 20px;

  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: flex-start;

  border-radius: 2px;
  border: 1px solid #eedfe0;
  background-color: rgba(238, 223, 224, 0.4);
}

.img-container {
  /* margin-top: 20px;
    margin-left: 20px; */

  width: 240px;
  height: 240px;

  display: flex;
  flex-direction: row;
  justify-content: center;

  border-radius: 2px;
  background-color: #ffffff;
}

.good-card__img {
  height: 240px;
  /* border-radius: 2px; */
  object-fit: cover;
}

.stars {
  width: 136px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  padding-top: 30px;
  padding-left: 52px;
}

/* .stars:hover {
  background-image: url("../assets/svg/black-star.svg");
  background-repeat: 5;
  background-position: center center;
} */

.stars__star {
  width: 24px;
  /* background-image: url("../assets/svg/black-star.svg"); */
}

.stars__star:hover {
  background-image: url("../assets/svg/black-star.svg");
  background-repeat: no-repeat;
  background-position: center center;
}

.good-info {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  padding-left: 20px;
}

.good-info__name {
  margin: 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 28px;

  color: #323232;
}

.price {
  margin: 0;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
}

.price__tittle {
  margin: 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 23px;

  color: #323232;
}

.price__price {
  margin: 0;
  margin-left: 10px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 23px;

  padding-top: 20px;
  padding-bottom: 20px;
  color: #323232;
}

.good-info__info {
  margin: 0;
  width: 345px;
  height: 150px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;

  color: #323232;
}

.card-buttons__button {
  margin: 0;
  width: 150px;
  height: 30px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;

  border: solid 0;
  border-radius: 2px;

  margin-right: 30px;
  margin-top: 30px;
  background-color: #eedfe0;
  color: #323232;
}

.card-buttons__button:hover {
  background-color: #d7576d;
  color: #eedfe0;
}
</style>
<template>
  <div class="main-background">
    <header-menu></header-menu>

    <div class="background">
      <div class="container">
        <div class="goods-page">
          <div class="filter">
            <img src="./assets/svg/filter.svg" class="filter__img" alt="" />
            <p class="filter__tittle">Фильтр</p>
          </div>

          <div class="goods">
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
            <good-card></good-card>
          </div>
        </div>

        <choose-page></choose-page>
      </div>
    </div>
    <footer-links></footer-links>
  </div>
</template>

<script>
import HeaderMenu from "./components/HeaderMenu.vue";
import GoodCard from "./components/GoodCard.vue";
import ChoosePage from "./components/ChoosePage.vue";
import FooterLinks from "./components/FooterLinks.vue";

export default {
  name: "App",
  components: {
    HeaderMenu,
    GoodCard,
    ChoosePage,
    FooterLinks,
  },

  // data() {
  //   return {
  //     WeatherForecast: [], //здесь - в массиве - будут отрисованы значения
  //     price: "cloud",
  //     cityName: null,
  //   }:
  // },

  //   methods: {
  //     UpdateData(data);

  //   },
  //   ApiLoad(lat, lon) {
  //     let url = new URL("")
  //     url.searchParams.set("lat", lat);

  //   fetch('https://fakestoreapi.com/products?limit=100')
  //     .then(res =>res.json())
  //     .then((json) => {
  //       this.WeatherForecast = json;
  //     }),
  //   },
  //   mounted() {
  //     console.log(1);
  //     //обращение к API ассинхронное
  //     this.ApiLoad(45.4112, -75.6981);
  //   },
};
</script>

<style>
#app {
  font-family: Roboto;
  /* -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}
/* @font-face {
  font-family: "Roboto";
  src: url("./assets/fonts/Roboto-Regular.ttf");
} */
body {
  margin: 0;
}

.main-background {
  background-color: #eedfe0;
}

.background {
  margin: 0 auto;
  width: 1400px;
  background-color: #fdf9f9;
}

.filter {
  width: 123px;

  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  padding-top: 30px;
  padding-bottom: 30px;
}

.filter__img {
  width: 30px;
}

.filter__tittle {
  margin: 0;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;

  color: #323232;
}

.goods {
  display: grid;
  grid-gap: 30px;
  grid-template-columns: repeat(auto-fill, 645px);
}
</style>

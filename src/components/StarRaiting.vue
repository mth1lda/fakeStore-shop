<template>
  <div class="rating_block">
    <input name="rating" value="5" id="rating_5" type="radio" />
    <label for="rating_5" class="label_rating"></label>

    <input name="rating" value="4" id="rating_4" type="radio" />
    <label for="rating_4" class="label_rating"></label>

    <input name="rating" value="3" id="rating_3" type="radio" />
    <label for="rating_3" class="label_rating"></label>

    <input name="rating" value="2" id="rating_2" type="radio" />
    <label for="rating_2" class="label_rating"></label>

    <input name="rating" value="1" id="rating_1" type="radio" />
    <label for="rating_1" class="label_rating"></label>
  </div>
</template>

<style scoped>
.rating_block {
  margin-top: 20px;
  margin-left: 57.5px;
  width: 125px;
  height: 25px;
}

.rating_block input[type="radio"] {
  display: none;
}

.label_rating {
  float: right;
  display: block;
  width: 25px;
  height: 25px;
  background: url(../assets/svg/star.svg) no-repeat 50% 0;
  cursor: pointer;
}

.rating_block .label_rating:hover,
.rating_block .label_rating:hover ~ .label_rating,
.rating_block input[type="radio"]:checked ~ .label_rating {
  background-position: 50% -25px;
  background: url(../assets/svg/black-star.svg) no-repeat 50% 0;
}
</style>
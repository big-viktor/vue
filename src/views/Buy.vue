<template>
  <div class="top_header">
    <div>
      <Back />
    </div>
    <div class="container_avatar">
      <Avatar />
    </div>
    <div></div>
  </div>

  <BreadCrumbs leftBread="#216 Snow Horse" />
  <Price Price="Price 120,000 USD" />

  <div class="container_list_card">
    <div class="content_list_cardItem">
      <div class="overf_card_list">
        <img
          :src="repo.src"
          class="img_listCard"
          v-for="repo in repos"
          :key="repo.name"
        />
      </div>
      <bayCard PriceBay="$900" Available="9211" Price="$300 for 0.1%" />
      <div class="">
        <p></p>
        <Buttons nameBtn="PAY" />
        <p></p>
      </div>
      <sliderChark />
    </div>
  </div>
</template>
<script>
// @ is an alias to /src

import Avatar from "../components/Avatar.vue";
import Back from "../components/Back.vue";
import BreadCrumbs from "../components/BreadCrumbs.vue";
import Price from "../components/Price.vue";
import Buttons from "../components/Buttons.vue";
import bayCard from "../components/bayCard.vue";
import sliderChark from "../components/sliderChark.vue";

export default {
  name: "Home",
  components: {
    Avatar,
    Back,
    BreadCrumbs,
    Price,
    Buttons,
    bayCard,
    sliderChark,
  },

  data() {
    return {
      repos: [
        { name: "test1", src: require("../assets/image1.png") },
        { name: "test1", src: require("../assets/Rectangle15.png") },
        { name: "test1", src: require("../assets/Rectangle23.png") },
        { name: "test1", src: require("../assets/Rectangle24.png") },
      ],
    };
  },
};
</script>
<style>
body {
  background-image: url("../assets/glav.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
.container_list_card {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
}
.content_list_card {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  width: 325px;
  margin: 10px 0px;
}
.img_listCard {
  width: 296px;
  height: 416px;
  padding: 0px 5px;
}
.top_header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 25px;
}
.container_avatar {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-left: 30px;
}

div {
  height: 100%;
}
@media (min-width: 660px) {
  .container_list_card {
    padding-top: 30px;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    flex-wrap: wrap;
    align-items: flex-start;
  }
}
.overf_card_list {
  padding-top: 10px;
  overflow-x: scroll;
  width: 325px;
  display: flex;
  flex-direction: row;
}
</style>

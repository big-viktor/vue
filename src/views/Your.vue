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

  <BreadCrumbs leftBread="BtehYYjefhw74hUUhc..." />
  <BreadCrumbs leftBread="Your Items" />

  <div class="container_list_card">
    <div v-for="repo in repos" :key="repo.name" class="content_list_card">
      <img :src="repo.src" class="img_list" />
      <Card
        nameCard="Art #221"
        namePrice="25,000 USD"
        nameAvailable="310/10000 available"
        img-Url="product.imgUrl"
      />
    </div>
  </div>
</template>
<script>
// @ is an alias to /src

import Avatar from "../components/Avatar.vue";
import Back from "../components/Back.vue";
import Card from "../components/card.vue";
import BreadCrumbs from "../components/BreadCrumbs.vue";

export default {
  name: "Home",
  components: {
    Avatar,
    Back,
    Card,
    BreadCrumbs,
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
.img_list {
  width: 100%;
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
</style>

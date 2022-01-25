<template>
  <div class="container_itemCard">
    <div class="Price_bay">
      {{ PriceBay }}
    </div>
    <div class="container_infoCard">
      <div class="title_card">Available:</div>
      <div class="text_card_title">{{ Available }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">Price:</div>
      <div class="text_card_title">{{ Price }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "bayCard",
  props: ["PriceBay", "Available", "Price"],
};
</script>

<style scoped>
.container_itemCard {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 325px;
}
.container_infoCard {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.Price_bay {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 36px;
  line-height: 42px;
  color: #000000;
  margin: 35px 0px;
}
.title_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: 500;
  font-size: 24px;
  line-height: 147.69%;
  color: rgba(0, 0, 0, 0.69);
}
.text_card_title {
  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 147.69%;
  color: rgba(0, 0, 0, 0.596);
}
</style>

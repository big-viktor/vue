<template>
  <div class="container_itemCard">
    <div class="info">
      {{ info }}
    </div>
    <div class="container_infoCard">
      <div class="title_card">Size:</div>
      <div class="text_card_title">{{ Size }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">Address:</div>
      <div class="text_card_title">{{ Address }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">IPFS:</div>
      <div class="text_card_title">{{ IPFS }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">Owner:</div>
      <div class="text_card_title">{{ Owner }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">Location:</div>
      <div class="text_card_title">{{ Location }}</div>
    </div>
    <div class="container_infoCard">
      <div class="title_card">Contributors:</div>
      <div class="text_card_title">{{ Contributors }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ItemCard",
  props: [
    "info",
    "Size",
    "Address",
    "IPFS",
    "Owner",
    "Location",
    "Contributors",
  ],
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
.info {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 23px;
  text-align: left;
  color: rgba(0, 0, 0, 0.596);
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

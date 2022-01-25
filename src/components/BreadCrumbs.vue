<template>
  <div class="container_bread">
    <div class="leftBread">{{ leftBread }}</div>
    <div class="rightBread">{{ rightBread }}</div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["leftBread", "rightBread"],
};
</script>

<style scoped>
.container_bread {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 10px 35px;
}
.rightBread {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 26px;
  line-height: 30px;
  color: #000000;
}
.leftBread {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 26px;
  line-height: 30px;

  color: #000000;
}
.container_card {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  background: #ffffff;
  border-radius: 4px;
  border-top: 0px;
  padding: 20px;
}
.name_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 28px;

  color: #000000;
}
.price_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 26px;
  line-height: 30px;
  color: #000000;
}
.avaiblable_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: 300;
  font-size: 22px;
  line-height: 26px;
  color: #000000;
}
</style>

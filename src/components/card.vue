<template>
  <div class="container_card">
    <p class="name_card">
      {{ nameCard }}
    </p>
    <p class="price_card">
      {{ namePrice }}
    </p>
    <p class="avaiblable_card">
      {{ nameAvailable }}
    </p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["nameCard", "namePrice", "nameAvailable"],
};
</script>

<style scoped>
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
  margin: 5px;
  color: #000000;
}
.price_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 26px;
  line-height: 30px;
  color: #000000;
  margin: 5px;
}
.avaiblable_card {
  font-family: Roboto;
  font-style: normal;
  font-weight: 300;
  font-size: 22px;
  line-height: 26px;
  color: #000000;
  margin: 5px;
}
</style>

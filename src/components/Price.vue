<template>
  <div class="">
    <div class="price">
      {{ Price }}
    </div>
  </div>
</template>

<script>
export default {
  name: "ItemCard",
  props: ["Price"],
};
</script>

<style scoped>
.price {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 26px;
  line-height: 30px;
  color: rgba(0, 0, 0, 0.596);
  text-align: left;
  padding-left: 30px;
}
</style>

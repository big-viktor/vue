<template>
  <div class="top_header">
    <div>
      <Back />
    </div>
    <div class="container_avatar">
      <Avatar />
    </div>
    <div>
      <Button nameBtn="Connect" />
    </div>
  </div>
  <div class="text">Connect your Wallet Solana</div>
  <div class="text_4">Without KYC</div>
  <div class="container_grup_btn">
    <div class="top_btn">
      <Button nameBtn="Buy part of Arts" />
    </div>
    <div class="top_btn">
      <whiteBtn nameBtnWite="Sell and Trade" />
    </div>
    <div class="top_btn">
      <whiteBtn nameBtnWite="Forum and comments" />
    </div>
    <div class="top_btn">
      <whiteBtn nameBtnWite="Add your Arts" />
    </div>
    <div class="text_4">I have read terms and conditions</div>
    <div class="top_btn">
      <Button nameBtn="Connect" />
    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import Button from "../components/Buttons.vue";
import Avatar from "../components/Avatar.vue";
import Back from "../components/Back.vue";
import whiteBtn from "../components/whiteBtn.vue";

export default {
  name: "Home",
  components: {
    Button,
    Avatar,
    Back,
    whiteBtn,
  },
};
</script>
<style>
.container_grup_btn {
  padding: 0px 45px;
}
.top_btn {
  padding-top: 20px;
}
body {
  background-image: url("../assets/glav.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
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
.text {
  font-family: Prompt;
  font-style: normal;
  font-weight: 300;
  font-size: 34px;
  line-height: 106.2%;
  text-align: center;
  color: #000000;
  max-width: 500px;
  padding-top: 60px;
}
.text_4 {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 26px;
  line-height: 30px;
  text-align: center;
  color: rgba(0, 0, 0, 0.69);
  padding-top: 30px;
}
div {
  height: 100%;
}
@media (min-width: 767px) {
  .container_grup_btn {
    display: flex;
    padding: 0px 45px;
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>

<template>
  <div class="bacg_N1">
    <div class="top_header">
      <div></div>
      <div class="container_avatar">
        <Avatar />
        <div class="text">
          Welcome to the first Solana NFT marketplace of real-world art objects
        </div>
        <div class="content_btn">
          <Button nameBtn="Browse all Arts" />
        </div>
      </div>
      <div class="content_btn_conect">
        <Button nameBtn="Connect" />
      </div>
      <div class="img_mob_menu">
        <img src="../assets/menu.png" alt="#" />
      </div>
    </div>
    <Slider />
  </div>
  <div class="bacg_N2">
    <div class="text2">Atmosphera</div>
    <div class="container_info">
      <div>
        <div class="text_3">
          Buy some part of real Arts, buy and sell tokens
        </div>
        <div class="text_3">
          Best auction for galleries and private collector
        </div>
      </div>
      <img src="../assets/Group26.png" alt="#" class="img_info_block" />
    </div>
    <div class="white_btn">
      <whiteBtn nameBtnWite="Learn more" />
    </div>
    <div class="content_footer">
      <Footer />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Button from "../components/Buttons.vue";
import Avatar from "../components/Avatar.vue";
import Slider from "../components/Slider.vue";
import whiteBtn from "../components/whiteBtn.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Home",
  components: {
    Button,
    Avatar,
    Slider,
    whiteBtn,
    Footer,
  },
};
</script>
<style>
.content_footer {
  padding-top: 170px;
}
.white_btn {
  max-width: 300px;
  margin: 0 auto;
  padding-top: 120px;
}
.text_3 {
  font-family: Prompt;
  font-style: normal;
  font-weight: normal;
  font-size: 30px;
  line-height: 106.2%;
  color: #ffffff;
  text-align: left;
  max-width: 383px;
  padding-top: 20px;
}
.container_info {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  padding: 0px;
  margin: 0px;
  background-color: black;
  background-size: 100%;
  background-repeat: no-repeat;
}

.bacg_N1 {
  position: relative;
  width: 100%;
  background-image: url("../assets/i1.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  height: 100%;
}
.top_header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-right: 65px;
  padding-left: 65px;
  padding-top: 80px;
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
.content_btn {
  padding-top: 70px;
}

.container_avatar {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-left: 70px;
}
.text2 {
  font-family: Prompt;
  font-style: normal;
  font-weight: normal;
  font-size: 77px;
  line-height: 116px;
  color: rgba(255, 255, 255, 0.21);
  text-align: left;
}
.bacg_N2 {
  margin: 0 auto;
  max-width: 705px;
}
.img_mob_menu {
  display: none;
}
@media (max-width: 735px) {
  .img_mob_menu {
    display: none;
  }
  .container_info {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-content: center;
  }
  .bacg_N2 {
    margin: 0 auto;
    max-width: 705px;
    padding: 50px 40px;
  }
  .img_info_block {
    width: 240px;
    height: 240px;
    display: flex;
    align-self: center;
    padding-top: 60px;
  }
  @media (min-width: 475px) {
    .img_mob_menu {
      display: none;
    }
  }
  @media (max-width: 475px) {
    .content_btn_conect {
      display: none;
    }
    .img_mob_menu {
      display: block;
    }
    .text2 {
      font-size: 55px;
    }
    .text3 {
      font-size: 30px;
    }
    .top_header {
      padding-right: 40px;
      padding-left: 40px;
    }
  }
}
</style>

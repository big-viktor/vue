<template>
  <div class="top_header">
    <div>
      <Back />
    </div>
    <div class="container_avatar">
      <Avatar />
    </div>
  </div>
  <div class="container_grup_btn">
    <div class="text_contact">Contacts</div>
    <p>New Arbat 21, 722</p>
    <p>Sales office: New Arbat 21, 722</p>
    <p>8 800 322 32 32</p>
  </div>
</template>
<script>
// @ is an alias to /src

import Avatar from "../components/Avatar.vue";
import Back from "../components/Back.vue";

export default {
  name: "Home",
  components: {
    Avatar,
    Back,
  },
};
</script>
<style>
.text_contact {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 32px;
  line-height: 37px;
  text-align: left;
  color: #000000;
}
.container_grup_btn {
  padding: 0px 45px;
}
.container_grup_btn p {
  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 26px;
  line-height: 30px;
  text-align: left;
  color: #000000;
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

<template>
  <div class="container_slider">
    <div class="top_img1 content_img">
      <img alt="slider" src="../assets/Rectangle15.png" class="img" />
      <img alt="slider" src="../assets/Rectangle24.png" class="img" />
    </div>
    <div class="top_img content_img">
      <img alt="slider" src="../assets/Rectangle16.png" class="img" />
      <img alt="slider" src="../assets/Rectangle20.png" class="img" />
    </div>
    <div class="content_img top_img3">
      <img alt="slider" src="../assets/Rectangle17.png" class="img" />
      <img alt="slider" src="../assets/Rectangle21.png" class="img" />
    </div>
    <div class="content_img top_img4">
      <img alt="slider" src="../assets/Rectangle18.png" class="img" />
      <img alt="slider" src="../assets/Rectangle22.png" class="img" />
    </div>
    <div class="content_img top_img5">
      <img alt="slider" src="../assets/Rectangle19.png" class="img" />
      <img alt="slider" src="../assets/Rectangle23.png" class="img" />
    </div>
  </div>
</template>

<style slider>
.content_img {
  display: flex;
  flex-direction: column;
}
.img {
  padding: 10px;
}
.top_img {
  margin-bottom: 90px;
}
.top_img1 {
  margin-top: 90px;
}
.top_img3 {
  margin-top: 50px;
}
.top_img4 {
  margin-top: 85px;
}
.top_img5 {
  margin-top: 105px;
}
.container_slider {
  display: flex;
  flex-direction: row;
  justify-content: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding-top: 100px;
}
@media (max-width: 1200px) {
  .container_slider {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 0 auto;
    padding-top: 100px;
    overflow-x: scroll;
    padding-left: 330px;
    width: 320px;
  }
}
@media (max-width: 670px) {
  .container_slider {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 0 auto;
    padding-top: 100px;
    overflow-x: scroll;
    padding-left: 350px;
    max-width: 200px;
  }
  .img {
    width: 170px;
    height: 220px;
  }
}
@media (max-width: 575px) {
  .container_slider {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 0 auto;
    padding-top: 100px;
    overflow: scroll;
    padding-right: 0px;
    width: 1px;
    padding-left: 370px;
  }
  .img {
    width: 130px;
    height: 190px;
  }
}
</style>

<template>
  <div class="container_footer">
    <img alt="Vue logo" src="../assets/avatar.png" class="img_fotter" />
    <p>Legal</p>
    <p>Contacts</p>
    <p>Terms of Service</p>
    <p>Privacy Policy</p>
  </div>
</template>

<style FOOTER>
.container_footer {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  font-family: Prompt;
  font-style: normal;
  font-weight: 300;
  font-size: 26px;
  line-height: 106.2%;
  color: #ffffff;
}
@media (max-width: 475px) {
  .container_footer {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    font-family: Prompt;
    font-style: normal;
    font-weight: 300;
    font-size: 26px;
    line-height: 106.2%;
    color: #ffffff;
  }
  .container_footer p {
    margin: 0px;
  }
  .img_fotter {
    margin-bottom: 60px;
  }
}
</style>

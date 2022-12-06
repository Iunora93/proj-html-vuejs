<script>
export default {
  name: "FooterBottom",  
};
</script>

<template>          
  <img src="../assets/imgSpa/avada-spa-logo-retina-new-200x23.png" alt="">
  <div class="copyright">
    <small>COPYRIGHT 2012-2020</small>
    <small>AVADA THEME BY THEMEFUSION</small>
    <small>ALL RIGHT RESERVED</small>
    <small>POWERED BY WORDPRESS</small>
  </div>
  <div class="icons">
    <i class="fa-brands fa-facebook-f"></i>
    <i class="fa-brands fa-twitter"></i>
    <i class="fa-brands fa-instagram"></i>
    <i class="fa-brands fa-youtube"></i>
  </div>


</template>

<style lang="scss" scoped>
.copyright{
  max-width: 30%;
  text-align: center;
  color: gray;
}
.icons{
  display: flex;
  justify-content: space-around;
  width: 25%;
  
  i{
    padding: 10px;
  background-color: lightgray;
  border-radius: 5px;
  color: gray;
  }
}
</style>
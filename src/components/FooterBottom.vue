<script>
export default {
  name: "FooterBottom",  
};
</script>

<template>          
  <img src="../assets/imgSpa/avada-spa-logo-retina-new-200x23.png" alt="">
  <div class="copyright">
    <small><a href="#">COPYRIGHT 2012-2020</a></small>
    |
    <small><a href="#">AVADA THEME BY THEMEFUSION</a></small>
    |
    <small><a href="#">ALL RIGHT RESERVED</a></small>
    |
    <small><a href="#">POWERED BY WORDPRESS</a></small>
  </div>
  <div class="icons">
    <button type="button"><i class="fa-brands fa-facebook-f"></i></button>
    <button type="button"><i class="fa-brands fa-twitter"></i></button>
    <button type="button"><i class="fa-brands fa-instagram"></i></button>
    <button type="button"><i class="fa-brands fa-youtube"></i></button>
  </div>


</template>

<style lang="scss" scoped>
.copyright{
  max-width: 30%;
  text-align: center;
  color: gray;
  font-size: 12px;
  small{
    margin: 0 5px;
    a{
      text-decoration: none;
      color: gray;
    }
  }
}
.icons{
  display: flex;
  justify-content: space-around;
  width: 25%;
  button{
  border: none;
  i{
    padding: 10px;
    background-color: rgb(229, 228, 228);
    border-radius: 5px;
    color: rgb(200, 198, 198);
  }
}
}
</style>
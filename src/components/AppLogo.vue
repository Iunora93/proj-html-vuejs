<script>
export default {
  name: "AppLogo",
  data() {
    return {
      logo: "avada-spa-logo-new.png",
    };
  },
  
};
</script>
<template>  
  <img :src="`/src/assets/imgSpa/${logo}`" alt="Logo" />
</template>
<style lang="scss">
    img{
    height: 25px;
    width: auto;
    }
</style>
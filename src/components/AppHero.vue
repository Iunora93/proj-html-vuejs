<script>
export default {
  name: "AppHero",  
};
</script>
<template>  
  <div class="hero">
    <div class="container">
        <h3><i>Give yourself permission</i></h3>
        <h1>Relax, Revive & Rejuvenate</h1>
        <button type="button">EXPLORE TREATMENTS</button>
    </div>    
  </div>
</template>
<style lang="scss">
    .hero{
    background-image: url(../assets/imgSpa/avada-spa-slider-image-1-new.jpg);
    padding: 50px 0 50px 0;
        .container{
            padding-top: 300px;
            padding-bottom: 350px;
            color: white;
            text-align: center;
                h1{
                    font-size: 68px;
                    margin: 50px 0 50px 0;
                }
                button{
                    border: none;
                    padding: 20px 50px;
                    border-radius: 50px;
                    background-color: #b9afa1;
                    color: white;                   
                    font-size: 16px;
                }
        }
    }
</style>
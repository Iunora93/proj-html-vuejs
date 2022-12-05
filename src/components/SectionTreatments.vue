<script>
export default {
  name: "SectionTreatments",
};
</script>
<template>  
<section>
  <div class="container">
    <div class="col-left">
        <img src="../assets/imgSpa/face_and_body_treatments-new-400x581.jpg" alt="">
    </div>
    <div class="col-right">
        <h1>Face & Body Treatments</h1>
        <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque, porro? Quod sunt nostrum excepturi commodi facilis consequuntur iusto voluptatum voluptatem ipsam, natus iste possimus aspernatur, necessitatibus atque quaerat tenetur laborum.</span>
    </div>
  </div>
</section>
</template>
<style lang="scss" scoped>
div{
    background-color: #f9f9f9;
    display: flex;
    padding: 50px 0;
}
img{
    border: solid 20px white;
    // box-shadow: 10px 10px 10px 10px black;
    margin: 20px;
    -moz-box-shadow: 10px 10px 10px #ccc;  
    box-shadow: 10px 10px 10px #ccc;  
}
.col-right{
    flex-direction: column;
}
    
</style>
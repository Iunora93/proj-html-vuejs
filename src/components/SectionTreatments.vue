<script>
export default {
  name: "SectionTreatments",
};
</script>
<template>  
<div>
  <div class="container">
    <div class="col-left">
        <img src="../assets/imgSpa/face_and_body_treatments-new-400x581.jpg" alt="">
    </div>
    <div class="col-right">
        <h1>Face & Body Treatments</h1>
        <span>Pellentesque nec felis efficitur, sagittis eros et, pharetra risus. Sed at lacus a ex imperdiet dignissim vehicula quam. Vestibulum ante ipsum primis.</span>
        
        <div class="box-treatments">
            <div class="treatments">
                <i class="fa-solid fa-plus"></i>
                <span>Oil Massage</span>
            </div>
            <div class="treatments">
                <i class="fa-solid fa-plus"></i>
                <span>Manicure</span>
            </div>
            <div class="treatments">
                <i class="fa-solid fa-plus"></i>
                <span>Aromatherapy</span>
            </div>
        </div>
        <button type="button"><a href="#">BOOK AN APPOINTMENT</a></button>
    </div>
  </div>
</div>
</template>
<style lang="scss" scoped>
div{
    background-color: #f9f9f9;
    display: flex;
    padding: 50px 0;
}
img{
    border: solid 20px white;
    margin: 20px;
    -moz-box-shadow: 10px 10px 10px #ccc;  
    box-shadow: 10px 10px 10px #ccc;  
}
.col-right{
    flex-direction: column;
    margin-top: auto;
    margin-bottom: auto;
    padding-left: 50px;
    padding-right: 50px;
    h1{
        font-size: 40px;
        color: #6f727b;
    }
    button{
        border: 2px solid #b9afa1;
        padding: 15px 30px;
        border-radius: 50px;
        background-color: inherit;
        color: #b9afa1;
        font-size: 16px;
        margin-right: auto;
        &:hover{
        
        border-color: #33a7b9;
      }
    a{
      text-decoration: none;
      color: #b9afa1;
      &:hover{
        color:  #33a7b9;
        
      }
    }   
  }
  .box-treatments{
    display: flex;
    flex-direction: column;
    
    .treatments{
        border: solid 1px #b9afa1;
        padding-left: 15px;
        margin-bottom: 10px;
        i{
            color: white;
            background-color: #6f727b;
            padding: 5px;
            margin-right: 15px;
        }
        span{
            font-style: italic;
            color: #b9afa1;
        }
    }
  }
}
    
</style>
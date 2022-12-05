<script>
export default {
  name: 'AppMain',
}
</script>

<template>
  <div class="container-small">
    <h1>Luxury Spa Experiences</h1>
    <i class="fa-solid fa-leaf"></i>
    <span><i>Morbi pharetra, quam id consequat imperdiet, lectus est tincidunt massa, eu posuere leo nibh non fermentum</i></span>
    <hr>
    <span class="intro">Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat volutpat. Fusce laoreet mi leo. Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat volutpat. Fusce laoreet mi leo.</span>
    <button type="button"><a href="#">OUR APPROACH</a></button>
  </div>
  <div class="container">
    <div class="icon-top">
      <i class="fa-solid fa-hands"></i>
      <div>Massages</div> 
    </div>
    <div class="icon-bottom">
      <i class="fa-regular fa-face-smile"></i>
      <div>Therapy</div>
    </div>
    <div class="icon-top">
      <i class="fa-solid fa-heart"></i>
      <div>Relaxing</div>
    </div>
    <div class="icon-bottom">
      <i class="fa-regular fa-moon"></i>
      <div>Meditation</div>
    </div>
    <div class="icon-top">
      <i class="fa-solid fa-snowflake"></i>
      <div>Natural Beauty</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container-small{  
  text-align: center;
  display: flex;
  flex-direction: column;
  padding: 20px;
  h1{
    color: #6f727b;    
  }
  span{
    padding-left:100px;
    padding-right:100px;
    color: #6f727b
  }
  i{
    color: #b9afa1;
    margin: 20px;
  }
  hr{  
    border: none;
    padding: 1px;
    background-color: #b9afa1;
    margin: 20px 45% 20px 45%;
  }
  .intro{
    font-size: 12px;
  }
  button{
    margin: 20px 30% 20px 30%;
    border: none;
    border: 2px solid #b9afa1;
    padding: 15px 30px;
    border-radius: 50px;
    background-color: white;
    color: #b9afa1;                   
    font-size: 16px;
    
    a{
      text-decoration: none;
      color: #b9afa1;
      &:hover{
        color:  #33a7b9;
        border-color: #33a7b9;
      }
    }   
  }
  
}
.container{
  display: flex;
  justify-content: space-between;
  text-align: center;
  height: 120px;
  margin-top: 20px;
  i{
    color: #b9afa1;
    font-size: 40px;
    margin-bottom: 20px;
  }
  .icon-bottom{
    margin-top: auto;
  }
  .icon-top, .icon-bottom{
    div{
      color: #6f727b;
    }
  }
}
</style>
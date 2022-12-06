<script>
import FooterBottom from "./FooterBottom.vue";
export default {
  name: 'AppFooter',
  components:{
    FooterBottom,
  },
  
}
</script>

<template>
  <footer>
    <div class="footer-top">
      <div class="container-small">
        <i>"If you want to relax, watch the clouds pass by if you're laying on the grass, or sit in front of the creek; just doing nothing and having those still moments is what really rejuvenates the body...""</i>
        <h3>FRIEDA FRIEDSON, MASSEUSE</h3>
      </div>
    </div>

    <div class="footer-center">
      <div class="container offer">
        <div class="special-offer">25%</div>
        <div class="discount">
          <h3>Take some time. Treat yourself. You deserve it.</h3>
          <span>Book a treatment this month and receive a 25% on all further treatments.</span>
        </div>
      </div>
      <button type="button">BOOK NOW</button>
    </div>

    <div class="footer-bottom">
     <FooterBottom /> 
    </div>
    
  </footer>
</template>

<style lang="scss" scoped>
.footer-top{
  background-image: url(../assets/imgSpa/Home-quota-new.jpg);
  padding: 300px;
  color: white;
  text-align: center;
  .container-small{
    
    h3{
      margin: 30px 0;
    }
  }
}
.footer-center{
  background-image: url(../assets/imgSpa/ptb_cta-new.jpg);
  padding: 50px;
  color: white;
  text-align: center;
  display: flex;
  border-bottom: 4px solid lightgray;
  .offer{
    display: flex;
    margin: auto;
    justify-content: space-between;
    text-align: left;
    .special-offer{
      font-size: 50px;
      border: 1px solid rgb(192, 175, 152);
      padding: 10px 20px 20px 20px;
      margin-right: 20px;
    }
    .discount{
        margin: auto;
        h3{
          margin-bottom: 10px;
        }
        span{
          font-size: 12px;
        }
      }
  }
  button{
    margin-right: auto;
    margin-top: auto;
    margin-bottom: auto;
    border: none;
    padding: 20px 50px;
    border-radius: 50px;
    background-color: #b9afa1;
    color: white;
    font-weight: bold;
    font-size: 16px;
    &:hover{
    background-color: #33a7b9;
    }
  }
}
.footer-bottom{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px;
}
</style>
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
        <div>
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
    padding: 0 100px;
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
  }
}
.footer-bottom{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px;
}
</style>
<script>
import AppLogo from "./AppLogo.vue";

export default {
  name: 'AppHeader',
  components: {
    AppLogo,
    
  },
  data() {
    return {
      links: [
        {
          icon: `<i class="fa-solid fa-feather"></i>`,
          href: "#",
          label: "TREATMENTS",
          info: 'Face & body',
        },
        {
          href: "#",
          
          icon: `<i class="fa-solid fa-person"></i>`,
          label: "ABOUT",
          info: 'Our Team',
        },
             
      ],
      lists: [
        {
          href: "#",
          icon: `<i class="fa-solid fa-heart"></i>`,
          label: "JOURNAL",
          info: 'Tips & Tricks',
        },
        {
          href: "#",
          icon: `<i class="fa-solid fa-bookmark"></i>`,
          label: "BOOK NOW",
          info: 'Special Offers',
        },   
      ],
    };
  },
}
</script>

<template>
  <header class="container">   
    <nav class="main-nav">
      <ul>
        <i class="fa-solid fa-house-chimney"></i>
        <li v-for="(item, index) in links">     
          <span v-html="item.icon"></span>     
          <a :href="item.href">{{ item.label }}</a>
          <h6>{{item.info}}</h6>
        </li>
      </ul>
      <AppLogo />
      <ul>
        <li v-for="(item, index) in lists">
          <span v-html="item.icon"></span>
          <a :href="item.href">{{ item.label }}</a>
          <h6>{{item.info}}</h6>
        </li>
        <i class="fa-solid fa-plus"></i>
      </ul>
    </nav>
  </header>
  
</template>

<style lang="scss" scoped>
header {
  text-align: center;
  margin-bottom: 3.125rem;
  padding: 50px;
  margin: auto;
  .main-nav {
    display: flex;
    
    ul {
      display: flex;      
      list-style: none;
      li{
        
        span{
          color: #b9afa1;
          
        }
      }
      
      i, a {
        display: inline-block;
        padding: 5px 25px;
        text-decoration: none;
        color: #6f727b;
       
      }
      i{
        margin: auto;
        color: #b9afa1;
          &:hover{
            color: #33a7b9;
          }
      }
      h6{
        color: #c0c1c5;
      }
    }
  }
}
</style>

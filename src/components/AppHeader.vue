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
          href: "#",
          label: "TREATMENTS",
          info: 'Face & body',
        },
        {
          href: "#",
          label: "ABOUT",
          info: 'Our Team',
        },
             
      ],
      lists: [
        {
          href: "#",
          label: "JOURNAL",
          info: 'Tips & Tricks',
        },
        {
          href: "#",
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
          <a :href="item.href">{{ item.label }}</a>
          <h6>{{item.info}}</h6>
        </li>
      </ul>
      <AppLogo />
      <ul>
        <li v-for="(item, index) in lists">
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

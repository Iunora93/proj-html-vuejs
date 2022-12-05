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
          label: "Home",
          info: 'face and body',
        },
        {
          href: "#",
          label: "Prodotti",
          info: 'face and body',
        },
        {
          href: "#",
          label: "Chi Siamo",
          info: 'face and body',
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
        
        <li v-for="(item, index) in links">
          <i class="fa-solid fa-house-chimney"></i>
          <a :href="item.href">{{ item.label }}</a>
          <small>{{item.info}}</small>
        </li>
      </ul>
      <AppLogo />
      <ul>
        <li v-for="(item, index) in links">
          <a :href="item.href">{{ item.label }}</a>
          <small>{{item.info}}</small>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss">
header {
  text-align: center;
  margin-bottom: 3.125rem;
  .main-nav {
    display: flex;
    ul {
      display: flex;
      list-style: none;
      justify-content: center;
      a {
        display: inline-block;
        padding: 15px 25px;
        text-decoration: none;
        color: #000;
       
      }
    }
  }
}
</style>

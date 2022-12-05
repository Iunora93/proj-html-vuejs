<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <div class="container">
    <AppHeader />
  </div>
  <div class="container-small">
    container small app vue
  </div>
  <AppMain />
  <AppFooter />

</template>

<style lang="scss">
@import './style/global.scss';
</style>

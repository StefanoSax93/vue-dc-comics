<template>
  <div id="app">
    <TheNavbar/>
    <BannerBlue/>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheNavbar from './components/TheNavbar.vue'
import TheFooter from './components/TheFooter.vue'
import BannerSignUp from './components/BannerSignUp.vue'
import BannerBlue from './components/BannerBlue.vue'

export default {
  name: 'App',
  components: {
    TheNavbar,
    TheFooter,
    BannerSignUp,
    BannerBlue
  }
}
</script>

<style lang="scss">
@import "assets/scss/main.scss";
@import "assets/scss/variables.scss";
@import url('https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;500;600;700&family=Montserrat:wght@100;200;300;400;500;600;700&display=swap');

#app {
  font-family: Asap Condensed, sans-serif;
}
</style>

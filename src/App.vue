<template>
  <div id="app">
    <TheNavbar/>
    <TheSlider/>
    <BannerBlue/>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheNavbar from './components/TheNavbar.vue'
import TheSlider from './components/TheSlider.vue'
import TheFooter from './components/TheFooter.vue'
import BannerSignUp from './components/BannerSignUp.vue'
import BannerBlue from './components/BannerBlue.vue'

export default {
  name: 'App',
  components: {
    TheNavbar,
    TheFooter,
    BannerSignUp,
    BannerBlue,
    TheSlider
}
}
</script>

<style lang="scss">
@import "./assets/scss/main.scss";
@import url('https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;500;600;700&family=Montserrat:wght@100;200;300;400;500;600;700&display=swap');

#app {
  font-family: Asap Condensed, sans-serif;
}
</style>

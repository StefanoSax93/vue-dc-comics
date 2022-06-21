<template>
  <div>
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

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

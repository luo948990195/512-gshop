<template>
  <div id="app">
    <router-view/>
    <footerGuide/>
  </div>
</template>

<script>
import footerGuide from './components/footerGuide/footerGuide.vue'
export default {
  name: 'App',
  components: {
    footerGuide
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
#app 
  width 100%
  height 100%
  background #f5f5f5

</style>

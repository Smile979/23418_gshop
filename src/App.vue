<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide v-show="$route.meta.showFooter"/>  
    <!--$route代表当前路由  -->
  </div>
</template>

<script>
  import FooterGuide from './components/FooterGuide/FooterGuide.vue'
  export default {
    components:{
      FooterGuide
    }
  }
</script>

<style lang="less">
  .app {
    width: 100%;
    height: 100%;
    background-color: #f5f5f5;
  }
</style>

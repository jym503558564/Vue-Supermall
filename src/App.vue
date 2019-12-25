<template>
  <div id="app">
    <router-view></router-view>
    <main-tabbar></main-tabbar>

  </div>
</template>

<script>
  import MainTabbar from 'components/content/maintabbar/MainTabbar'
  import "assets/css/base.css";
  export default {
    name: 'app',
    components: {
      MainTabbar
    }
  }
</script>

<style>
</style>

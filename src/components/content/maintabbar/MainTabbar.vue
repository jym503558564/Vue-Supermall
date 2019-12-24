<template>
  <tab-bar>
    <tabbar-item path="/home">
      <div slot="item-icon" class="iconfont icon-shouye"></div>
      <div slot="item-text">首页</div>
    </tabbar-item>
    <tabbar-item path="/category">
      <div slot="item-icon" class="iconfont icon-fenlei"></div>
      <div slot="item-text">分类</div>
    </tabbar-item>
    <tabbar-item path="/cart">
      <div slot="item-icon" class="iconfont icon-gouwuche"></div>
      <div slot="item-text">购物车</div>
    </tabbar-item>
    <tabbar-item path="/profile">
      <div slot="item-icon" class="iconfont icon-wode"></div>
      <div slot="item-text">我的</div>
    </tabbar-item>
  </tab-bar>
</template>

<script>
  import TabBar from 'components/common/tabbar/Tabbar'
  import TabbarItem from "components/common/tabbar/TabbarItem";
  export default {
    name: "MainTabbar",
    components:{
      TabBar,
      TabbarItem
    }
  }
</script>

<style scoped>

</style>
<template>
  <div :class="{is_active: is_active}" class="tab-bar-item" @click="itemClick">
    <slot name="item-icon"></slot>
    <slot name="item-text"></slot>
  </div>
</template>

<script>
  export default {
    name: "TabbarItem",
    props:{
      path: String,
    },
    data(){
      return {
        // is_active: true

      }
    },
    computed:{
      is_active(){
        return this.$route.path.indexOf(this.path) !== -1
      }
    },
    methods: {
      itemClick(){
        this.$router.push(this.path)
      },
    }
  }
</script>

<style scoped>
  @import "~assets/css/tabbar/iconfont.css";
  .tab-bar-item {
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14px;
  }
  .is_active{
    color: deeppink;
  }
</style>
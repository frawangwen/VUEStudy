<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item path="/home" activeColor="blue">
        <img slot="item-icon" src="./assets/img/tabbar/home.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/home_active.svg"
          alt=""
        />
        <div slot="item-text">首页</div>
      </tab-bar-item>

      <tab-bar-item path="/category" activeColor="blue">
        <img slot="item-icon" src="./assets/img/tabbar/category.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/category_active.svg"
          alt=""
        />
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/cart" activeColor="blue">
        <img slot="item-icon" src="./assets/img/tabbar/shopcart.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/shopcart_active.svg"
          alt=""
        />
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile" activeColor="blue">
        <img slot="item-icon" src="./assets/img/tabbar/profile.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/profile_active.svg"
          alt=""
        />
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
//导入组件
import TabBar from "./components/tabber/TabBar.vue";
import TabBarItem from "./components/tabber/TarBarItem.vue";

export default {
  name: "App",
  //注册组件
  components: {
    TabBar,
    TabBarItem,
  },
};
</script>

<style scope>
/* 在样式中引用CSS文件要用@import */
@import "./assets/css/base.css";
</style>

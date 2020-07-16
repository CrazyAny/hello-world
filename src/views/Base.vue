<template>
  <div class="home">
    <el-container>
      <!-- 这是头部的开始 -->
      <el-header id="header">       
        <el-menu
          :default-active="activeIndex2"
          class="el-menu-demo"
          mode="horizontal"
          @select="handleSelect"
          background-color="#545c64"
          text-color="#fff"
          active-text-color="#ffd04b">
          <el-menu-item index="1"><router-link to="/">首页</router-link></el-menu-item>
          <el-menu-item index="2"><router-link to="/qurey">办公用品查询</router-link></el-menu-item>
          <el-menu-item index="3">办公用品申请</el-menu-item>
          <el-menu-item index="4">办公用品录入</el-menu-item>
         
        </el-menu>
      </el-header>
      <!-- 这是头部的结束 -->
      <!-- 这是主体的开始 -->
      <el-main id="main">
        <slot name="main"><Carousel></Carousel></slot>
      </el-main>
      <!-- 这是主体的结束 -->
      <!-- 这是尾部的开始 -->
      <el-footer>Footer</el-footer>
      <!-- 这是尾部的结束 -->
    </el-container>
  </div>
</template>
<script>
import Carousel from '@/components/Carousel.vue'
  export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    },
    components:{Carousel}

  }
</script>
<style scoped >
#el-meun-1{
  /* margin-top: -50px; */
  position: relative;
  
}
#header{
  padding: 0 0;
}
#main{
  height: 800px;
  padding: 0;
}
a {
  text-decoration: none;
}
 
.router-link-active {
  text-decoration: none;
}
</style>
<template>
  <div class="block">
    
    <el-carousel height="550px">
      <el-carousel-item v-for="item in url" :key="item">
        <img :src="item" alt="图片加载错误" height="650px">
      </el-carousel-item>  
    </el-carousel>
  </div>

</template>
<script>
export default {
    name:'Carousel',
    data(){
        return{
            url:['Carousel/img1.jpg','Carousel/img2.jpg','Carousel/img3.jpg','Carousel/img4.jpg','Carousel/img5.jpg','Carousel/img6.jpg',],
        }
    }
}
</script>
<style >
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
  }

  .el-carousel__item:nth-child(2n) {
     background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
     background-color: #d3dce6;
  }
</style>

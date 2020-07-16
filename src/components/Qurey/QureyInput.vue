<template>

<el-form :inline="true" :model="formInline" class="demo-form-inline ">
  <el-form-item label="编号查询">
    <el-input v-model="formInline.user" placeholder="请输入编号"></el-input>
  </el-form-item>
  <el-form-item label="名称查询">
    <el-input v-model="formInline.user" placeholder="请输入物品名称"></el-input>
  </el-form-item>
  <el-form-item>
    <el-button type="primary" @click="onSubmit">查询</el-button>
  </el-form-item>
</el-form>

</template>
<script>
  export default {
    data() {
      return {
        formInline: {
          user: '',
          region: ''
        }
      }
    },
    methods: {
      onSubmit() {
        console.log('submit!');
      }
    }
  }
</script>
<style lang="less" scoped>
// .demo-form-inline{
//     margin-top: 20px;
    
    
// }
</style>
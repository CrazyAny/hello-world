<template>
  <div>
    <base-nav >
      <div slot="main" class="main">
        <div class="qurey-input">
          <qurey-input>
          </qurey-input>
          <qurey-data></qurey-data>    
        </div>    
      </div>
    </base-nav>
  </div>
</template>
<script>
import BaseNav from '@/views/Base.vue'
import QureyInput from '@/components/Qurey/QureyInput.vue'
import QureyData from '@/components/Qurey/QureyData.vue'
export default {
    name:'Qurey',
    components:{
        BaseNav,QureyInput,QureyData
    }
}
</script>
<style lang="less" scoped>
.main{
    margin: 10px 0px;
    text-align: left;
    .qurey-input{
    display: inline-block;
}
}
</style>
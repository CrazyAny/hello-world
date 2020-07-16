<template>
    <div class="qurey-data" id="qurey-data">
        <ul>
            <li>物品编号</li>
            <li>名称</li>
            <li>规格型号</li>
            <li>数量</li>
            <li>单价</li>
            <li>总价</li>
            <li>采购日期</li>
            <li>录入日期</li>
        </ul>
    </div>
</template>
<style lang="less" scoped>
.qurey-data{
    
    text-align: center;
    ul{
        li{ 
            display: inline-block;
            text-decoration: none;
            list-style: none;
            border: 1px solid black;
            box-sizing: border-box;
            width: 100px;
            height: 50px;
            line-height: 50px;
            text-align: center;
            
        }
    }
}

</style>
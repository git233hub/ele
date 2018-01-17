<!--首页下面的头部-->  
<!--scoped不跟其他页面样式冲突-->
<template>
<header class="header">
    <div>福中三路深圳市民中心</div>
    <div>
        搜索商家,商品名称
    </div>
</header>
</template>

<script>
export default {
    name: 'home-header'
}
</script>

<style scoped>      
    .header{
        width: 100%;
        height: 80px;
        background-image: linear-gradient(90deg,#0af,#0085ff);
    }
</style>

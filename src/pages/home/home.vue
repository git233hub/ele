<template>
<div>
  <!--首页面-->
  <page pageId="home">
    <home-header></home-header>
    <home-banner></home-banner>
    <home-list></home-list>  
  </page> <!--子页面不要装在这个结构了-->
<!--两个同级标签不能放在一个template中-->
  <router-view></router-view><!--子页面-->
</div>
</template>

<script>
import page from '../../common/page.vue'  //引入page组件
import header from '../../components/home/index/header.vue';
import banner from '../../components/home/index/banner.vue';
import list from '../../components/home/index/list.vue';
export default {
  //声明有哪些组件
  components:{
    [page.name]:page,
    [header.name]:header,
    [banner.name]:banner,
    [list.name]:list,
  }
}
</script>

<style>

</style>

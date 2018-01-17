<template>
<div class="page" :id="pageId" ref="page">
    <div class="wrapper"> 
        <slot></slot>
    </div> 
</div>
</template>

<script>
import IScroll from 'iscroll';
// console.log(IScroll);
export default {
    name: 'page',
    props: {
        pageId: String
    },
    mounted(){   //mounted  才有dom结构   created中 没有
                                    //第一个参数是选择器
        let pageScroll = new IScroll(this.$refs.page, {
            
        });
    }
}
</script>

<style>
.page{
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 49px;
    overflow: hidden;
}
</style>

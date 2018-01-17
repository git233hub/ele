<template>
<div class="subpage" :id="pageId">
    <slot></slot> 
</div>
</template>

<script>
// import IScroll from 'iscroll';
// console.log(IScroll);
export default {
    name: 'sub-page',
    props: {    
        pageId: String
    },
    // mounted(){
    //     let pageScroll = new IScroll(this.$refs.page, {

    //     });
    // }
}
</script>

<style>
.subpage{
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0px;
    
    z-index:2
}
</style>

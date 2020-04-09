<template>
   <div id="MainBlock" class="row">
       <SideBar class="col-1-of-4"/>
       <ContentBlock class="col-3-of-4"/>
       
   </div>
</template>

<script>
    import SideBar from './SideBar.vue'
    import ContentBlock from './ContentBlock.vue'
    
    export default {
        name: 'mainblock',
        components: {
            SideBar,
            ContentBlock
        }
    }

</script>

<style>

</style>

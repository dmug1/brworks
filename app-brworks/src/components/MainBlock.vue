<template>
   <div id="MainBlock">
       <SideBar/>
       <ContentBlock/>
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
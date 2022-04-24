<template>
    <div class="container">
       <div class="row">
           
           <div class="col-sm-4 bg-dark">
               <left-navbar />
           </div>

           <div class="col-sm-8 bg-light border-start">
               <right-navbar />
           </div>
           <hr>
       </div>
    </div>
</template>

<script>
    import LeftNavbar from './LeftNavbar.vue'
    import RightNavbar from './RightNavbar.vue'
    export default {
        name:'MainNavbar',
        components:{
            LeftNavbar,
            RightNavbar
        }
    }
</script>

<style lang="scss" scoped>

</style>

<template>
    <div class="container mt-3 ">
        <div class="w-100 p-2 " id="vueTopHeader">
            <span class=" "> Vue3 is now the new default version! </span>
            <router-link class="inside-block text-white" to="/about">Learn More</router-link>
        </div>
        <h1>this component were been simulated from vuejs.org main pages.</h1>
        <h2>This page edit from github pages....</h2>
    </div>
</template>

<script>
    export default {
        name:'VueOrg'
    }
</script>

<style lang="scss" scoped>
#vueTopHeader{
    background-color: rgba(29, 236, 150, 0.63);
    color: white;
}

</style>

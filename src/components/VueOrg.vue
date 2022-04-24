<template>
    <div class="container mt-3 ">
        <div class="w-100 p-2 " id="vueTopHeader">
            <span class=" "> Vue3 is now the new default version! </span>
            <router-link class="inside-block text-white" to="/about">Learn More</router-link>
        </div>
        <main-navbar />
    </div>
</template>

<script>
import MainNavbar from "./MainNavbar.vue"

    export default{
        name:'VueOrg',

        components: {
            MainNavbar
        }
    }
</script>

<style lang="scss" scoped>
#vueTopHeader{
    background-color: rgba(29, 236, 150, 0.63);
    color: white;
}

</style>

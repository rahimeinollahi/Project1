<template>
    <div class="container-mt-1">
        <div class="row">
            <div class="col-sm-8">

            </div>
        </div>
        <ul class="nav nav-pills mt-2">
            <li class="nav-item dropdown">
                <a href="#" class="nav-link text-dark dropdown-toggle" data-bs-toggle="dropdown">Docs</a>
                <ul class="dropdown-menu">
                    <li v-for="item in docItems"
                    :key="item.id">
                        <router-link class="dropdown-item" to="/about">{{item.name}}</router-link>
                    </li>
                </ul>
            </li>
            <li class="nav-item">
                <router-link class="nav-link text-dark" to="/apiroute">API</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link text-dark" to="/apiroute">Playground</router-link>
            </li>

            <li class="nav-item dropdown">
                <a class="nav-link text-dark dropdown-toggle" data-bs-toggle="dropdown" src="#">Ecosustem</a>
                <ul class="dropdown-menu">
                    <li v-for="item2 in playgroundItems"
                    :key="item2.id">
                        <router-link v-if="item2.id!=8" class="dropdown-item" :to="item2.path">{{item2.name}}</router-link>
                        
                        <div v-else>
                            <hr>
                        <router-link v-for="item3 in item2.name2" :key="item3.id"  class="dropdown-item" :to="item3.path">{{item3.name2}}</router-link>
                        </div>
                    </li>
                </ul>
            </li>

            <li class="nav-item dropdown">
                <a class="nav-link text-dark dropdown-toggle" href="#" data-bs-toggle='dropdown'>About</a>
                <ul class="dropdown-menu">
                    <li v-for="item4 in aboutItems"
                    :key="item4.id">
                        <router-link class="dropdown-item" :to="item4.path">{{item4.name}}</router-link>
                    </li>
                </ul>
            </li>
            <li class="nav-item">
                <router-link class="nav-link text-dark" to="/sponser">Sponser</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link text-dark" to="/">Partnes</router-link>
            </li>
        </ul>
    </div>
</template>

<script>
    // import NavRightIcon from './NavRightIcon.vue'
    export default {
        components:{
            // NavRightIcon
        },
        name:'RightNavbar',
        data(){
            return{
                docItems:[
                    {id:1,name:'Tuturial',path:'/'},
                    {id:2,name:'Example',path:'/'},
                    {id:3,name:'Quick Start',path:'/'},
                    {id:4,name:'Styel Guid',path:'/'},
                    {id:5,name:'Migration: from vue2 ',path:'/'},
                ],
                playgroundItems:[
                    {id:1,name:'Resources',path:'/'},
                    {id:2,name:'Partnes',path:'/'},
                    {id:3,name:'Themes',path:'/'},
                    {id:4,name:'Jobs',path:'/'},
                    {id:5,name:'T-Shirt-shop',path:'/'},
                    {id:6,name:'Core Libraries',path:'/'},
                    {id:7,name:'Pinia',path:'/'},

                    {id:8,name2:[
                        {id:81,name2:'Video Courses',path:'/'},
                        {id:82,name2:'Vue mastery',path:'/'},
                        {id:83,name2:'Vue School',path:'/'},
                    ]},
                ],
                aboutItems:[
                    {id:1,name:'FAQ',path:'/'},
                    {id:2,name:'Team',path:'/'},
                    {id:3,name:'Release',path:'/'},
                    {id:4,name:'Community-Guid',path:'/'},
                    {id:5,name:'Code-of-Counter',path:'/'},
                    {id:6,name:'The Documentary',path:'/'},
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>
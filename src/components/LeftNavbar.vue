<template>
    <nav class="navbar navbar-expand-sm navbar-light bg-light">
  <div class="container-fluid">
    <!-- <a class="navbar-brand" href="javascript:void(0)">Logo</a> -->
    <img src="../assets/logo.png" alt="vuejs-logo" id="logo-navbar" class="">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mynavbar">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="mynavbar">
      <ul class="navbar-nav me-auto">
        <li class="nav-item">
          <!-- <a class="nav-link" href="javascript:void(0)">Vuejs</a> -->
          <router-link class="nav-link" to="/vuejs-nav">Vuejs</router-link>
        </li>
        <li class="nav-item">
            <kbd class="text-white bg-secondary e-2 mx-2 ">ctrl+k</kbd>          
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="text" placeholder="Search">
        <button class="btn btn-light border" type="button">Search</button>
      </form>
    </div>
  </div>
</nav>

</template>

<script>
    export default {
        name:'LeftNavbar'
    }
</script>

<style lang="scss" scoped>
#logo-navbar{
    width: 30px;
    height: 30px;
}
</style>
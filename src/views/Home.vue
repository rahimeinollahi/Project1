<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <main-navbar />
    <h1 class="text-success">The progressive</h1>
    <h2>JavaScript Framework</h2>
    <h5 class="text-dark">An approachable, performant and versatile framework for building web user interfaces.</h5>

      <button class="btn btn-lg btn-success me-2">Why vue</button>
      <button class="btn btn-lg btn-light me-2">Why vue</button>
      <button class="btn btn-lg btn-light me-2">Why vue</button>

      <hr>
        <div class="d-felx justify-content-center">
            <span class="mx-2 inline-block">Special Sponser</span>
            <span class="mx-2 inline-block">HBuilder</span>
            <span class="mx-2 inline-block">Advanced IDE for vue</span>
        </div>
      <hr>

      <div class="row">

        <div class="col-sm-4  flex-cloumn justify-content-center">
            <h4>Approachable</h4>
            <p class="text-center">Builds on top of standard HTML, CSS and JavaScript with intuitive API and world-class documentation.</p>
        </div>

        <div class="col-sm-4 flex-cloumn">
          <h4>Performant</h4>
          <p>Truly reactive, compiler-optimized rendering system that rarely requires manual optimization.</p>
        </div>

        <div class="col-sm-4">
          <h4 class="flex-coloumn">versatile</h4>
          <p>A rich, incrementally adoptable ecosystem that scales between a library and a full-featured framework.</p>
        </div>
      </div>
      <h3 class="d-flex justify-content-start">Platinum Sponser</h3>

      <div class="row d-flex justify-content-center ">
        
          <div class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">
            <img src="../assets/logo.png" class="rounded" alt="button-logo" style="width:50px" height="50px">
            <button class="btn btn-light btn-lg">Vue School</button>
          </div>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">Vehicle</button>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">passionante pople</button>
        
      </div>
      <div class="row d-flex justify-content-center ">

          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">Storyblok</button>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">ionic</button>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">Nuxt js</button>
        
      </div>
      <div class="row d-flex justify-content-center ">

          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">Refuerbed</button>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">ButterCMS</button>
          <button class="btn btn-lg btn-light col-sm-3 mx-2 border p-3 mt-3">your logo</button>
        
      </div>

      <div class="row mt-3">
        <div class="d-flex justify-content-center">
        <div class="col-sm-3"></div>
        <div class="col-sm-6">
          <div class="row">
          <div class="col-sm border m-1 btn-lg">
                <img src="../assets/logo.png" alt="vuemaster-image">
                <button class="btn btn-light ">Vue mastery</button>
            </div>
            <div class="col-sm border m-1 btn-lg">
                <img src="../assets/logo.png" alt="vuemaster-image">
                <button class="btn btn-light ">Laravel</button>
            </div>
            <div class="col-sm border m-1 btn-lg">
                <img src="../assets/logo.png" alt="vuemaster-image">
                <button class="btn btn-light ">Html Burger</button>
            </div>
        </div>
        </div>
        <div class="col-sm-3"></div>
        </div>
      </div>
        <hr>

         <div class="row">
           <div class="col-sm-3"></div>
           <div class="col-sm-6">
             <p class="display-6 text-dark">Subscribe to our weekly newsletter</p>
             <div class=" d-flex border p-3 ">
               <input type="text" class="form-control">
               <button class="btn btn-lg btn-success mx-2">Subscribe</button>
             </div>
             <span>You can read the previous issues and listen to our podcast at </span>
                 <router-link to="/" class="text-success ">news.vuejs.org.</router-link><br>
                 <span class="mt-3">You may also go social at Twitter, or join our home at </span>
                 <router-link  to="/" class="text-success mt-3">Discord</router-link>
           </div>
           <div class="col-sm-3"></div>
         </div>
  </div>
   
</template>

<script>
// @ is an alias to /src
import MainNavbar from '@/components/MainNavbar.vue'

export default {
  name: 'Home',
  components: {
    MainNavbar
  }
}
</script>

<style lang="scss" scoped>
h1{
  font-size: 4rem;
  background-image: linear-gradient(to right,rgb(175, 252, 239),rgb(51, 190, 255));
}

h2{
  font-size: 6rem;
}
img{
  width: 50px;
  height: 50px;
}
</style>

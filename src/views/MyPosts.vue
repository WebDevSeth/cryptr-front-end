<template>
   <div class="container">
    <header
      class="
        d-flex
        flex-wrap
        align-items-center
        justify-content-center justify-content-md-between
        py-3
        mb-4
        border-bottom
      "
    >
      <a
        href="/"
        class="
          d-flex
          align-items-center

          mb-2 mb-md-0
          text-dark text-decoration-none
        "
      >
           <router-link  to="newPost" class="btn btn-sm btn-outline-secondary">
                +POST
              </router-link >

             <router-link to="/feeds" class="btn btn-sm btn-outline-secondary">BACK TO FEED</router-link>

        <img class="logo" src="../assets/logo.png" alt="" />
      </a>

      <div class="col-md-3 text-end">

          <router-link  to="Profile" class="btn btn-sm btn-outline-secondary">
                MY PROFILE
              </router-link >

     <router-link  to="/" class="btn btn-sm btn-outline-secondary">SIGN OUT</router-link>
      </div>
    </header>
  </div>

<br>
<br>
<br>



<!-- feed -->


  
</template>

<script>
export default {

}
</script>

<style scoped>

.cardtop {
  height: 150px !important;
  width: 150px !important;
  display: block !important;
  margin: auto !important;
}


.logo {
  left:48%;
  position:absolute !important;
height:55px !important;
width:55px !important;
}


</style>
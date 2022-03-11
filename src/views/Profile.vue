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
          col-md-3
          mb-2 mb-md-0
          text-dark text-decoration-none
        "
      >
        <img class="logo" src="../assets/logo.png" alt="" />
      </a>

      <div class="col-md-3 text-end">
             <router-link  to="/" class="btn btn-sm btn-outline-secondary">UPDATE MY PROFILE</router-link>

      <router-link  to="Feeds" class="btn btn-sm btn-outline-secondary">BACK TO FEEDS</router-link>
      </div>
    </header>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
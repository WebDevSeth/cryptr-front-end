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

       <router-link  to="MyPosts" class="btn btn-sm btn-outline-secondary">
                MY POSTS
              </router-link >

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


  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3 feeds">
    <div class="col" v-for="posts of post" :key="posts._id">
      <div class="card shadow-sm">
        <br />
        <div class="cardProf">
          <i class="bi bi-person-square"></i>
          <p>test</p>
        </div>
        <img
          class="cardtop"
          :src="posts.img">
      
        <div class="card-body">
          <p class="card-text">{{posts.description}}</p>
          <div class="d-flex justify-content-between align-items-center">
            <div class="btn-group">
              <button type="button" class="btn btn-sm btn-outline-secondary">
                COMMENT
              </button>
             
            </div>
             <button type="button" class="btn btn-sm btn-outline-secondary">
                BOOST
              </button>
           
          </div>
        </div>
      </div>
    </div>
  </div>





  
</template>

<script>
export default {
  data() {
    return {
      post: null,
    };
  },
  mounted() {
    fetch("https://socialmediacryptr.herokuapp.com/posts", {
      method: "GET",
      headers: {
        "Content-type": "application/json; charset=UTF-8",
      },
    })
      .then((response) => response.json())
      .then((json) => {
        this.post = json;
      })
      .catch((err) => {
        alert(console.log(err));
      });
  },
};
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
height:50px !important;
width:50px !important;
}


.btn {
  background-color: #008037 !important;
  color: white !important;

}


.card {
  background-color:white !important;
}

</style>
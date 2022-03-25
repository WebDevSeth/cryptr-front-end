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
        <router-link to="/feeds" class="btn btn-sm btn-outline-secondary"
          >BACK TO FEED</router-link
        >

        <img class="logo" src="../assets/logo.png" alt="" />
      </a>

      <div class="col-md-3 text-end">
        <router-link to="Profile" class="btn btn-sm btn-outline-secondary">
          MY PROFILE
        </router-link>

        <router-link to="/" class="btn btn-sm btn-outline-secondary"
          >SIGN OUT</router-link
        >
      </div>
    </header>
  </div>

  <br />
  <br />
  <br />

  <!-- new post button -->

  <button
    type="button"
    class="btn btn-primary"
    data-bs-toggle="modal"
    data-bs-target="#exampleModal"
  >
    +POST
  </button>

  <div
    class="modal fade"
    id="exampleModal"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <button
          type="button"
          class="btn-close"
          data-bs-dismiss="modal"
          aria-label="Close"
        ></button>

        <div class="modal-body">
          <div class="modal-content">
            <div class="modal-body">
              <div class="mb-3">
                <label for="addImg" class="form-label">Image URL</label>
                <input
                  class="form-control"
                  type="text"
                  name="addImg"
                  id="addImg"
                  v-model="img"
                />
              </div>
              <div class="mb-3">
                <label for="addDescription" class="form-label"
                  >Description</label
                >
                <input
                  class="form-control"
                  type="text"
                  name="addDescription"
                  id="addDescription"
                  v-model="description"
                />
              </div>
            </div>

      
            <br />
            <button
              type="button"
              class="btn btn-primary"
              data-bs-dismiss="modal"
              @click="createPost()"
            >
              Create Post
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    // Create Product
    createPost() {
      if (!localStorage.getItem("jwt")) {
        alert("User not logged in");
        return this.$router.push({ name: "Login" });
      }
      fetch("https://socialmediacryptr.herokuapp.com/posts", {
        method: "POST",
        // mode: "no-cors",
        body: JSON.stringify({
          description: this.description,
          img: this.img,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
          Authorization: `Bearer ${localStorage.getItem("jwt")}`,
        },
      })
        .then((response) => response.json())
        .then((json) => {
          alert("Post Created");
          this.$router.push({ description: "Posts" });
        })
        .catch((err) => {
          alert(err);
        });
    },

    
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
height:55px !important;
width:55px !important;
}

.btn {
  background-color: #008037 !important;
  color: white !important;

}

.card {
background-color: grey !important;

}
</style>
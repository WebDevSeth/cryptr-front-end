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

<div class="aboutpage">
    <div class="container cont">
      <div class="form">
        <form action="https://formspree.io/f/xzboabqr" method="POST"
>
          <label>Name:</label>
          <input type="name" v-model="name" required />


          <label>Email:</label>
          <input type="email" name="email" v-model="email" required />
          
          <label>Message:</label>
          <input type="message" name="message" v-model="message" required />
          <div class="submit" type="submit">
            <button class="submit1">Submit</button>
          </div>
        </form>
      </div>
    </div>
    </div>
  
</template>

<script>

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

form {
  max-width: 420px;
  margin-top: 50px !important;
  margin-bottom: 120px !important;
  margin: auto;
  background-color: grey !important;
  text-align: center;
  padding: 40px;
  border-radius: 10px;
  font-size: 22px !important;
}

label {
  color: black;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}

input,
select {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd !important;
  color: black !important;
  background: #ddd !important;
}
input[type="checkbox"] {
  display: inline-block;
  width: 16px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
button {
  background: #0d6efd !important;
  border: 0;
  padding: 10px 20px;
  margin-top: 20px;
  color: white !important;
  border-radius: 20px;
  cursor: pointer;
}
button:hover {
  opacity: 0.8;
}
.submit1 {
  text-align: center;
  background-color:green !important;
  
}
</style>
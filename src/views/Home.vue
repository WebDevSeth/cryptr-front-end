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
        <button onclick="document.getElementById('id02').style.display='block'">
          Login
        </button>
        <button onclick="document.getElementById('id01').style.display='block'">
          Sign Up
        </button>
      </div>
    </header>
  </div>
  <div class="home">
    <main>
      <div
        class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center"
      >
        <div class="col-md-5 p-lg-5 mx-auto my-5">
          <h1 class="display-4 fw-normal text-white">ABOUT CRYPTR</h1>
          <p class="lead fw-normal text-white">
            Post, like and comment on the<br />
            Cryptocurrency and NFTs you love.
          </p>
          <a
            class="btn btn-outline-secondary text-white"
            href="https://en.wikipedia.org/wiki/Cryptocurrency"
            target="_blank"
            >Learn more..</a
          >
        </div>
        <div class="product-device shadow-sm d-none d-md-block"></div>
        <div
          class="product-device product-device-2 shadow-sm d-none d-md-block"
        ></div>
      </div>
    </main>
  </div>

  <!-- The Modal (contains the Sign Up form) -->
  <div id="id01" class="modal">
    <span
      onclick="document.getElementById('id01').style.display='none'"
      class="close"
      title="Close Modal"
      >x</span
    >
    <form class="modal-content" action="/action_page.php">
      <div class="container">
        <h1>Sign Up</h1>

        <hr />
        <label for="email"><b>Email</b></label>
        <input type="text" placeholder="Email" name="email" required />

        <label for="psw"><b>Password</b></label>
        <input type="password" placeholder="Password" name="psw" required />

        <label>
          <input
            type="checkbox"
            checked="checked"
            name="remember"
            style="margin-bottom: 15px"
          />
          Remember me
        </label>

        <p>
          By creating an account you agree to our
          <a href="#" style="color: dodgerblue">Terms & Privacy</a>.
        </p>

        <div class="clearfix">
          <button
            type="button"
            onclick="document.getElementById('id01').style.display='none'"
            class="cancelbtn"
          >
            Cancel
          </button>
          <button type="submit" class="signup">Sign Up</button>
        </div>
      </div>
    </form>
  </div>

  <!-- login -->

  <!-- The Modal (contains the Sign Up form) -->
  <div id="id02" class="modal">
    <span
      onclick="document.getElementById('id02').style.display='none'"
      class="close"
      title="Close Modal"
      >x</span
    >
    <form class="modal-content" action="/action_page.php">
      <div class="container">
        <h1>LOGIN</h1>

        <hr />
        <label for="email"><b>Email</b></label>
        <input type="text" placeholder="Email" name="email" required />

        <label for="psw"><b>Password</b></label>
        <input type="password" placeholder="Password" name="psw" required />

        <label>
          <input
            type="checkbox"
            checked="checked"
            name="remember"
            style="margin-bottom: 15px"
          />
          Remember me
        </label>

        <p>
          By creating an account you agree to our
          <a href="#" style="color: dodgerblue">Terms & Privacy</a>.
        </p>

        <div class="clearfix">
          <button
            type="button"
            onclick="document.getElementById('id02').style.display='none'"
            class="cancelbtn"
          >
            CANCEL
          </button>
          <router-link  to="/feeds" class="signup">LOGIN</router-link>
        </div>
      </div>
    </form>
  </div>

  <br />
  <br />
  <br />
  <br />
  
  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
    <div class="col">
      <div class="card shadow-sm">
        <br />
        <div class="cardProf">
          <i class="bi bi-person-square"></i>
          <p>Exciller111</p>
        </div>
        <img
          class="cardtop"
          src="https://img.icons8.com/external-becris-lineal-color-becris/100/000000/external-blockchain-fintech-becris-lineal-color-becris.png"
        />
        <div class="card-body">
          <p class="card-text">This is a bla bla bla</p>
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
    <div class="col">
      <div class="card shadow-sm">
           <br />
        <div class="cardProf">
          <i class="bi bi-person-square"></i>
          <p>BananaBread420</p>
        </div>
        <img
          class="cardtop"
          src="https://img.icons8.com/cotton/64/000000/nft.png"
        />
        <div class="card-body">
          <p class="card-text">This is a bla bla bla</p>
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
    <div class="col">
      <div class="card shadow-sm">
           <br />
        <div class="cardProf">
          <i class="bi bi-person-square"></i>
          <p>SethTheCreator69</p>
        </div>
        <img
          class="cardtop"
          src="https://img.icons8.com/external-soft-fill-juicy-fish/60/000000/external-crypto-digital-nomad-soft-fill-soft-fill-juicy-fish.png"
        />
        <div class="card-body">
          <p class="card-text">This is a bla bla bla</p>
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
  <br />
  <br />
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
};
</script>


<style scoped>
.position-relative {
  background-image: url(../assets/bit.jpg);
}
.cardtop {
  height: 150px !important;
  width: 150px !important;
  display: block !important;
  margin: auto !important;
}

* {
  box-sizing: border-box;
}
/* Full-width input fields */
input[type="text"],
input[type="password"] {
  width: 100%;
  padding: 15px;
  margin: 5px 0 22px 0;
  display: inline-block;
  border: none;
  background: #f1f1f1;
}

/* Add a background color when the inputs get focus */
input[type="text"]:focus,
input[type="password"]:focus {
  background-color: #ddd;
  outline: none;
}

/* Set a style for all buttons */
button {
  background-color: #04aa6d;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 50%;
  opacity: 0.9;
}

button:hover {
  opacity: 1;
}

/* Extra styles for the cancel button */
.cancelbtn {
  padding: 14px 20px;
  background-color: #f44336;
}

/* Float cancel and signup buttons and add an equal width */
.cancelbtn,
.signupbtn {
  float: left;
  width: 50%;
}

/* Add padding to container elements */
.container {
  padding: 16px;
}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: #474e5d;
  padding-top: 50px;
}

/* Modal Content/Box */
.modal-content {
  background-color: #fefefe;
  margin: 5% auto 15% auto; /* 5% from the top, 15% from the bottom and centered */
  border: 1px solid #888;
  width: 80%; /* Could be more or less, depending on screen size */
}

/* Style the horizontal ruler */
hr {
  border: 1px solid #f1f1f1;
  margin-bottom: 25px;
}

/* The Close Button (x) */
.close {
  position: absolute;
  right: 35px;
  top: 15px;
  font-size: 40px;
  font-weight: bold;
  color: #f1f1f1;
}

.close:hover,
.close:focus {
  color: #f44336;
  cursor: pointer;
}

/* Clear floats */
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}

/* Change styles for cancel button and signup button on extra small screens */
@media screen and (max-width: 300px) {
  .cancelbtn,
  .signupbtn {
    width: 100%;
  }
}
</style>
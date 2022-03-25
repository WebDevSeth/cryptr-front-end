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
        <img class="logo " src="../assets/logo.png" alt="" />
      </a>

      <div class="col-md-3 text-end">
        <button class="btn btn-sm btn-outline-secondary" onclick="document.getElementById('id02').style.display='block'">
          Login
        </button>
        <button class="btn btn-sm btn-outline-secondary" onclick="document.getElementById('id01').style.display='block'">
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
            Post, and comment on the<br />
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
    <form @submit.prevent="register" class="modal-content">
      <div class="container">
        <h1>Sign Up</h1>

        <hr />

        <label for="email"><b>Full name</b></label>
        <input
          type="text"
          placeholder="Full name"
          name="email"
          v-model="fullname"
          required
        />

        <label for="email"><b>Phone number</b></label>
        <input
          type="text"
          placeholder="Phone number"
          name="email"
          v-model="phone_number"
          required
        />

        <label for="email"><b>Email</b></label>
        <input
          type="text"
          placeholder="Email"
          name="email"
          v-model="email"
          required
        />

        <label for="psw"><b>Password</b></label>
        <input
          type="password"
          placeholder="Password"
          name="psw"
          v-model="password"
          required
        />

        <label for="img"><b>Profile picture</b></label>
        <input
          type="img"
          placeholder="IMG URL"
          name="image"
          v-model="image"
          required
        />
        <br />
        <br />

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
            class="c-btn btn-sm"
          >
            Cancel
          </button>
          <button type="submit" class="btn btn-sm">
            Sign Up
          </button>
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
    <form class="modal-content"  @submit.prevent="login">
      <div class="container">
        <h1>LOGIN</h1>

        <hr />
        <label for="email"><b>Email</b></label>
        <input type="text" v-model="email" placeholder="Email" name="email" required />
 
        <label for="psw"><b>Password</b></label>
        <input type="password" v-model="password" placeholder="Password" name="psw" required />

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
            class="c-btn btn-sm"
          >
            CANCEL
          </button>
         <button type="submit" class="btn btn-sm">LOGIN</button>
        </div>
      </div>
    </form>
  </div>
<div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="../assets/Cara1.png" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="../assets/Cara2.png" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="../assets/Cara3.png" class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
    <div class="col">
      <div class="card">
        <br />
 
        <img
          class="cardtop"
          src="https://www.quoteinspector.com/media/bitcoin/tarnished-cryptocurrrency-coins-wo.jpg"
        />
        <div class="card-body">
          <p class="card-text">Eth is boosting, Lets go to the moon!</p>
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
  
        <img
          class="cardtop"
          src="https://everythinginclick.com/wp-content/uploads/2021/03/Facebooks-New-Cryptocurrency_-Libra.png"
        />
        <div class="card-body">
          <p class="card-text">Have you heard about Facebooks new cryptocurrency?</p>
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
  
        <img
          class="cardtop"
          src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fs3.tradingview.com%2Fc%2FCt7u2ia6_big.png&f=1&nofb=1"
        />
        <div class="card-body">
          <p class="card-text">Btc market is going down? what do you think</p>
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
// @ is an alias to /src

export default {
  data() {
    return {
      fullname: "",
      email: "",
      phone_number: "",
      password: "",
      image: "",
    };
  },
  methods: {
    register() {
      fetch("https://socialmediacryptr.herokuapp.com/users/", {
        method: "POST",
        body: JSON.stringify({
          fullname: this.fullname,
          email: this.email,
          phone_number: this.phone_number,
          password: this.password,
          image: this.image,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => {
          alert("User registered");
          localStorage.setItem("jwt", json.jwt);
          this.$router.push({ fullname: "Login" });
        })
    },

  

        login() {
      fetch("https://socialmediacryptr.herokuapp.com/users/", {
        method: "PATCH",
        body: JSON.stringify({
          email: this.email,
          password: this.password,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => {
          localStorage.setItem("jwt", json.jwt);
          alert("User logged in");
          this.$router.push({ name: "Feeds" });
        })
        .catch((err) => {
          alert("User does not exsist");
        });
    },

  },
};
</script>


<style scoped>

.c-btn {
  background-color: red !important;
  color: white !important;
}


.position-relative {
  background-image: url(../assets/bit.jpg);
}


.carousel-item {
  height: 850px !important

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

.carousel-control-prev-icon {

  background-color: black;
    border-radius:50%;
}

.carousel-control-next-icon {

  background-color: black;
  border-radius:50%;
}


/* Add a background color when the inputs get focus */
input[type="text"]:focus,
input[type="password"]:focus {
  background-color: #ddd;
  outline: none;
}

/* Set a style for all buttons */

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

.btn {
  background-color: #008037 !important;
  color: white !important;

}

.cardtop {
  height: 250px !important;
  width: 250px !important;
  display: block !important;
  margin: auto !important;
  border-radius: 5% !important;
}


.card {
  background-color: grey !important;
  color:white !important;
}



.logo {
  left:48%;
  position:absolute !important;
height:55px !important;
width:55px !important;
}




</style>
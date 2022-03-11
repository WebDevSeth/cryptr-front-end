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
           <button type="button" class="btn btn-sm btn-outline-secondary">
                +POST
              </button>

         <button type="button" class="btn btn-sm btn-outline-secondary">
                MY POSTS
              </button>

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

<!-- modal -->





<!-- feed -->


  
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
          src="https://img.icons8.com/ios-filled/50/000000/ethereum.png"/>
      
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
          src="https://img.icons8.com/color/48/000000/bitcoin--v1.png"/>

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

  <br>

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

  <br>

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
      margin: 0 auto !important;
  display: block !important;
  position: absolute !important;
  left: calc((100% - 195px) / 2);
  z-index: -100000 !important;
}

</style>
<template>
  <div class="hero">
    <!-- versi desktop -->
    <div class="v-desktop d-none d-md-block">
      <div class="row py-4">
        <div class="col-md-6">
          <div class="d-flex h-100">
            <div class="justify-content-center align-self-center">
              <h2>
                <strong>Delicious Food Menu, </strong> <br />
                In Your Gadget
              </h2>
              <p>Ayo segera pilih dan pesan makanan favorite Anda</p>
              <router-link class="btn btn-lg btn-success" to="/foods"
                ><b-icon-arrow-right></b-icon-arrow-right> Pesan</router-link
              >
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <img
            src="../assets/images/heroImage.svg"
            alt="Hero Image"
            width="100%"
          />
        </div>
      </div>
    </div>

    <!-- versi mobile -->
    <div class="v-mobile d-sm-block d-md-none">
      <div class="row py-4">
        <div class="col-md-6 mb-3">
          <img
            src="../assets/images/heroImage.svg"
            alt="Hero Image"
            width="100%"
          />
        </div>

        <div class="col-md-6">
          <div class="d-flex h-100">
            <div class="justify-content-center align-self-center">
              <h2>
                <strong>Delicious Food Menu, </strong> <br />
                In Your Gadget
              </h2>
              <p>Ayo segera pilih dan pesan makanan favorite Anda</p>
              <router-link class="btn btn-lg btn-success" to="/"
                ><b-icon-arrow-right></b-icon-arrow-right> Pesan</router-link
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>

<style>
</style>
<template>
  <div class="pesanan-sukses">
    <NavbarNav />
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col text-center">
          <img src="../assets/images/menunggu.png" width="300" />
          <h2>Sukses!!</h2>
          <h4>
            Pesanan Anda segera diproses <br />
            Selamat Menunggu
          </h4>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavbarNav from "@/components/NavbarNav.vue";

export default {
  name: "PesananSuksesView",
  components: {
    NavbarNav,
  },
};
</script>

<style>
</style>
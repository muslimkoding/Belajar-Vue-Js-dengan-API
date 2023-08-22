<template>
  <div class="home">
    <NavbarNav />
    <div class="container">
      <HeroSection />

      <div class="row mt-4">
        <div class="col">
          <h2>Best <strong>Foods</strong></h2>
        </div>

        <div class="col">
          <router-link class="btn btn-success float-right" to="/foods"
            ><b-icon-eye></b-icon-eye> Lihat Semua</router-link
          >
        </div>
      </div>

      <div class="row mb-3">
        <div
          class="col-md-4 mt-4"
          v-for="product in products"
          :key="product.id"
        >
          <CardProduct :product="product" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavbarNav from "@/components/NavbarNav.vue";
import HeroSection from "@/components/HeroSection.vue";
import CardProduct from "@/components/CardProduct.vue";
import axios from "axios";
export default {
  name: "HomeView",
  components: {
    NavbarNav,
    HeroSection,
    CardProduct,
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProducts(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3000/best-products")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log("Gagal :", error));
  },
};
</script>

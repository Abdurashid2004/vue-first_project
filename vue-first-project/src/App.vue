<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import BaseFilter from "./components/BaseFilter.vue";
import Products from "./components/Products.vue";
import Button from "./components/Button.vue";
import AboutSec from "./components/AboutSec.vue";
import BlogsSec from "./components/BlogsSec.vue";
import Blogs2 from "./components/Blogs2.vue";
import Login from "./components/Login.vue";
// import Footer from "./components/Footer.vue";

export default {
  components: {
    Navbar,
    Header,
    BaseFilter,
    Products,
    Button,
    AboutSec,
    BlogsSec,
    Blogs2,
    Login,
    // Footer,
  },
  methods: {
    showMadal() {
      this.isMadal = true;
    },
  },
};
</script>

<template>
  <div class="container">
    <Navbar @login-clicked="showMadal" />
    <Header />
    <div class="grid grid-cols-4 gap-8">
      <BaseFilter class="col-span-1" />
      <Products class="col-span-3" />
    </div>
    <Button />
    <AboutSec />
    <BlogsSec />
    <Blogs2 />
    <Login v-if="isMadal" @close="isMadal = false" />
    <div
      class="col-span-4 flex items-center gap-6 text-center h-10 py-8 justify-around bg-green-200 mb-5"
    >
      <img
        src="./assets/logo1.png"
        alt="Green Shop Logo"
        class="object-contain bg-green-200"
      />
      <h3 class="flex-1">70 West Buckingham Ave. Farmingdale, NY 11735</h3>
      <p class="flex-1">contact@greenshop.com</p>
      <p class="flex-1">+88 01911 717 490</p>
    </div>
    <!-- <Footer /> -->
  </div>
</template>

<style scoped></style>

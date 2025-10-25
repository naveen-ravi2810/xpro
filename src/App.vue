<template>
  <div>
    <Navbar />
    <Home />
    <BannerScroll />
    <About />
    <Supports />
    <Products />
    <Contact />
  </div>
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import About from "./views/About.vue";
import Home from "./views/Home.vue";
import Supports from "./views/Supports.vue";
import Contact from "./views/Contact.vue";
import Products from "./views/Products.vue";
import BannerScroll from "./views/BannerScroll.vue";
</script>

<template>
  <section class="relative py-12 bg-gray-50 overflow-hidden">
    <!-- Web: two columns with 3D scroll animation -->
    <div class="hidden md:grid md:gap-8 max-w-5xl mx-auto perspective-1000">
      <div
        v-for="(product, index) in products"
        :key="index"
        ref="webItems"
        class="relative rounded-xl shadow-xl overflow-hidden transform opacity-0 transition-all duration-700 will-change-transform hover-effect"
        :class="index % 2 === 0 ? 'rotate-left' : 'rotate-right'"
      >
        <img
          :src="product.image"
          :alt="product.name"
          class="w-full h-80 lg:h-96 object-cover"
        />
      </div>
    </div>

    <!-- Mobile: vertical scroll -->
    <div class="flex flex-col items-center space-y-12 px-4 md:hidden">
      <div
        v-for="(product, index) in products"
        :key="index"
        ref="mobileItems"
        class="w-full rounded-xl shadow-lg overflow-hidden transform translate-y-20 opacity-0 transition-all duration-700 hover:scale-105"
      >
        <img
          :src="product.image"
          :alt="product.name"
          class="w-full h-64 sm:h-80 object-cover"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import SunFilm from "@/assets/Banner1.png";
import ScreenGuard from "@/assets/Banner2.png";
import PPF from "@/assets/Banner3.png";
import Ceramic from "@/assets/Banner4.png";
import { onMounted, ref } from "vue";

const products = [
  { name: "Sun Film", image: SunFilm },
  { name: "Screen Guard", image: ScreenGuard },
  { name: "PPF (Paint Protection Film)", image: PPF },
  { name: "Nano Ceramic Safety Glazing Films", image: Ceramic },
];

const webItems = ref([]);
const mobileItems = ref([]);

onMounted(() => {
  const observerMobile = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.remove("translate-y-20", "opacity-0");
          entry.target.classList.add("translate-y-0", "opacity-100");
        }
      });
    },
    { threshold: 0.2 }
  );
  mobileItems.value.forEach((el) => observerMobile.observe(el));

  const observerWeb = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.remove(
            "rotate-left",
            "rotate-right",
            "opacity-0"
          );
          entry.target.classList.add("rotate-0", "opacity-100");
        }
      });
    },
    { threshold: 0.2 }
  );
  webItems.value.forEach((el) => observerWeb.observe(el));
});
</script>

<style scoped>
/* 3D perspective */
.perspective-1000 {
  perspective: 1000px;
}

/* Initial rotation for scroll-in effect */
.rotate-left {
  transform: rotateY(-25deg) translateX(-50px);
  opacity: 0;
}
.rotate-right {
  transform: rotateY(25deg) translateX(50px);
  opacity: 0;
}
.rotate-0 {
  transform: rotateY(0deg) translateX(0px);
  opacity: 1;
}

/* Hover effect for web */
.hover-effect:hover {
  transform: translateY(-10px) scale(1.05) rotateY(0deg);
  box-shadow: 0 25px 35px rgba(0, 0, 0, 0.25);
  transition: all 0.5s ease;
}

/* Hover scale for mobile */
.hover\:scale-105:hover {
  transform: scale(1.05) !important;
  transition: transform 0.3s ease;
}
</style>

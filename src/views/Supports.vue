<template>
  <section class="px-6 py-12 bg-gray-50">
    <h2
      class="text-3xl sm:text-4xl font-semibold mb-8 text-center text-gray-800"
    >
      Compatible With
    </h2>

    <div class="relative w-full overflow-hidden bg-gray py-6 rounded-xl">
      <!-- Animated Slider -->
      <div class="flex w-max animate-scroll gap-12">
        <img
          v-for="(logo, index) in extendedLogos"
          :key="index"
          :src="logo"
          class="h-20 sm:h-28 w-auto object-contain"
          alt="Car Brand Logo"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
const logos = [
  "https://rdoverseas.in/cdn/shop/files/toyota.webp",
  "https://rdoverseas.in/cdn/shop/files/mg.webp",
  "https://rdoverseas.in/cdn/shop/files/kia.webp",
  "https://rdoverseas.in/cdn/shop/files/mahindra.webp",
  "https://rdoverseas.in/cdn/shop/files/Maruti_Suzuki.webp",
  "https://rdoverseas.in/cdn/shop/files/Renault.webp",
  "https://rdoverseas.in/cdn/shop/files/ISUZU.webp",
  "https://rdoverseas.in/cdn/shop/files/CHE.webp",
];

// Duplicate array to create infinite scroll illusion
const extendedLogos = [...logos, ...logos];
</script>

<style scoped>
@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(
      -50%
    ); /* scroll half width because we duplicated logos */
  }
}

.animate-scroll {
  display: flex;
  gap: 3rem;
  animation: scroll 15s linear infinite;
}

@media (max-width: 640px) {
  .animate-scroll {
    animation-duration: 15s; /* slower on mobile */
  }
}
</style>

<template>
  <section class="px-6 py-12 bg-gray-50">
    <h2
      class="text-3xl sm:text-4xl font-semibold mb-12 text-center text-gray-800"
    >
      Our Products
    </h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 max-w-5xl mx-auto">
      <!-- Sun Film -->
      <div
        class="group bg-white rounded-xl shadow-lg overflow-hidden transform hover:scale-105 transition duration-300"
      >
        <img
          src="./../assets/SunFlim.png"
          alt="Sun Film"
          class="w-full h-64 object-contain p-4 bg-gray-50"
        />
        <h3 class="text-xl font-semibold text-gray-700 text-center py-4">
          Sun Film
        </h3>
      </div>

      <!-- Screen Guard -->
      <div
        class="group bg-white rounded-xl shadow-lg overflow-hidden transform hover:scale-105 transition duration-300"
      >
        <img
          src="./../assets/ScreenGuards.png"
          alt="Screen Guard"
          class="w-full h-64 object-contain p-4 bg-gray-50"
        />
        <h3 class="text-xl font-semibold text-gray-700 text-center py-4">
          Screen Guard
        </h3>
      </div>

      <!-- PPF (Paint Protection Film) -->
      <div
        class="group bg-white rounded-xl shadow-lg overflow-hidden transform hover:scale-105 transition duration-300"
      >
        <img
          src="./../assets/PPF.png"
          alt="PPF"
          class="w-full h-64 object-contain p-4 bg-gray-50"
        />
        <h3 class="text-xl font-semibold text-gray-700 text-center py-4">
          PPF (Paint Protection Film)
        </h3>
      </div>

      <!-- Nano Ceramic Safety Glazing Films -->
      <div
        class="group bg-white rounded-xl shadow-lg overflow-hidden transform hover:scale-105 transition duration-300"
      >
        <img
          src="./../assets/NanoCeramicSafetyGlazingFilms.png"
          alt="Nano Ceramic Safety Glazing Films"
          class="w-full h-64 object-contain p-4 bg-gray-50"
        />
        <h3 class="text-xl font-semibold text-gray-700 text-center py-4">
          Nano Ceramic Safety Glazing Films
        </h3>
      </div>
    </div>
  </section>
</template>

<script setup>
// No extra logic required
</script>

<style scoped>
/* Smooth hover effect with shadow */
.group:hover img {
  transform: scale(1.05);
  transition: transform 0.3s ease;
}
</style>

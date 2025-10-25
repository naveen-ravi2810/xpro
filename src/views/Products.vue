<template>
  <section class="px-6 py-12 bg-gray-50">
    <h2
      class="text-3xl sm:text-4xl font-semibold mb-8 text-center text-gray-800"
    >
      Our Products
    </h2>

    <div class="flex flex-col sm:flex-row gap-8 justify-center items-center">
      <!-- Sun Film -->
      <div class="flex-1 text-center">
        <img
          src="./../assets/SunFlim.png"
          alt="Sun Film"
          class="w-full sm:h-64 object-contain rounded-lg shadow-lg"
        />
        <h3 class="mt-4 text-xl font-medium text-gray-700">Sun Film</h3>
      </div>

      <!-- Screen Guard -->
      <div class="flex-1 text-center">
        <img
          src="./../assets/ScreenGuards.png"
          alt="Screen Guard"
          class="w-full sm:h-64 object-contain rounded-lg shadow-lg"
        />
        <h3 class="mt-4 text-xl font-medium text-gray-700">Screen Guard</h3>
      </div>
    </div>
  </section>
</template>

<script setup>
// No extra logic needed for now
</script>

<style scoped>
/* Optional: smooth hover effect */
img:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease;
}
</style>

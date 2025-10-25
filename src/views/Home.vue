<template>
  <div class="relative flex flex-col">
    <!-- Hero Section -->
    <section
      class="flex flex-col items-center justify-center text-center px-4 py-12 sm:py-16 bg-gray-50"
    >
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold text-gray-900">
        Protect. Enhance. Shine.
      </h2>
      <p
        class="mt-4 sm:mt-6 max-w-xl sm:max-w-2xl text-sm sm:text-base md:text-lg text-gray-600 leading-relaxed"
      >
        At <strong>X-Pro</strong>, we specialize in high-performance
        <span class="font-semibold text-yellow-600">Sunfilms</span> and
        <span class="font-semibold text-orange-500">Screen Guards</span>,
        crafted to keep your vehicles cool, stylish, and protected. We also
        offer
        <span class="font-semibold text-yellow-600"
          >PPF (Paint Protection Film)</span
        >
        to safeguard your car’s paint, and
        <span class="font-semibold text-orange-500"
          >Nano Ceramic Safety Glazing Films</span
        >
        for ultimate shine and protection. Our products deliver crystal-clear
        visibility, UV resistance, and lasting durability — engineered for
        perfection.
      </p>

      <!-- Friendly Customer Message -->
      <p class="mt-4 text-sm sm:text-base md:text-lg text-gray-700 font-medium">
        We are a
        <span class="text-yellow-600 font-semibold">friendly partner</span>
        for our lovable customers, guiding you to choose the best for your car.
      </p>
    </section>
  </div>
</template>

<style scoped>
/* Optional fine-tuning for hero on mobile */
@media (max-width: 640px) {
  h2 {
    font-size: 2rem;
  }

  p {
    font-size: 0.9rem;
    line-height: 1.4rem;
  }

  section {
    padding: 2rem 1rem;
  }
}
</style>

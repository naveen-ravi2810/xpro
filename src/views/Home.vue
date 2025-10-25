<template>
  <div class="relative flex flex-col min-h-screen">
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
        <strong>Sunfilms</strong> and <strong>Screen Guards</strong> crafted to
        keep your vehicles cool, stylish, and protected. Our products deliver
        crystal-clear visibility, UV resistance, and lasting durability —
        engineered for perfection.
      </p>
    </section>

    <!-- Banner Section -->
    <section class="w-full">
      <div class="w-full relative">
        <!-- Mobile: show full image -->
        <img
          src="@/assets/Banner1.png"
          alt="X-Pro Banner"
          class="block sm:hidden w-full h-auto object-contain"
        />
        <!-- Web: cinematic crop -->
        <img
          src="@/assets/Banner1.png"
          alt="X-Pro Banner"
          class="hidden sm:block w-full h-full"
        />
      </div>
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

<template>
  <div class="relative">
    <!-- About Us Section -->
    <section class="relative px-6 py-12 sm:py-16 bg-gray-50 overflow-hidden">
      <!-- Decorative background circle -->
      <div
        class="absolute -top-16 -left-16 w-64 h-64 bg-gradient-to-r from-yellow-200 to-yellow-400 rounded-full opacity-20"
      ></div>

      <div class="max-w-3xl mx-auto text-center space-y-6 animate-fadeIn">
        <h2 class="text-3xl sm:text-4xl font-bold text-gray-900">About Us</h2>
        <p class="text-gray-700 text-base sm:text-lg leading-relaxed">
          We are a
          <span class="font-semibold text-yellow-600"
            >dedicated manufacturing company</span
          >
          specializing in
          <span class="font-semibold text-orange-500"
            >high-quality automotive solutions</span
          >. With our
          <span class="font-semibold text-yellow-500"
            >own production facilities</span
          >, we ensure every product meets the
          <span class="font-semibold text-orange-500">highest standards</span>
          of performance and durability.
        </p>
        <p class="text-gray-700 text-base sm:text-lg leading-relaxed">
          Our expertise includes
          <span class="font-semibold text-yellow-600">premium sun films</span>
          for cars, designed to provide
          <span class="font-semibold text-orange-500"
            >superior heat rejection</span
          >, <span class="font-semibold text-yellow-500">UV protection</span>,
          and enhanced comfort for drivers and passengers. Additionally, we
          manufacture
          <span class="font-semibold text-orange-500"
            >precision-fit screen guards</span
          >
          for infotainment systems, protecting your vehicle’s display from
          scratches, smudges, and everyday wear.
        </p>
        <p class="text-gray-700 text-base sm:text-lg leading-relaxed">
          As a
          <span class="font-semibold text-yellow-600">stand-alone company</span
          >, we take pride in delivering
          <span class="font-semibold text-orange-500"
            >exceptional products</span
          >
          while maintaining strong
          <span class="font-semibold text-yellow-500"
            >customer satisfaction</span
          >. Our commitment to
          <span class="font-semibold text-orange-500"
            >quality, innovation, and service</span
          >
          sets us apart in the automotive accessory industry.
        </p>
      </div>
    </section>

    <!-- About Banner -->
    <section class="w-full">
      <img
        src="@/assets/Banner2.png"
        alt="X-Pro Banner"
        class="w-full h-auto object-cover"
      />
    </section>
  </div>
</template>

<style scoped>
/* Fade-in animation */
@keyframes fadeIn {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fadeIn {
  animation: fadeIn 1s ease-out forwards;
}

/* Responsive adjustments */
@media (max-width: 640px) {
  h2 {
    font-size: 2rem;
  }

  p {
    font-size: 0.95rem;
    line-height: 1.5rem;
  }
}
</style>

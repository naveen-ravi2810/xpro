<template>
  <div class="relative px-6 py-12 sm:py-16 bg-gray-50">
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
        <span class="font-semibold text-orange-500">highest standards</span>.
      </p>

      <p class="text-gray-700 text-base sm:text-lg leading-relaxed">
        Our products include
        <span class="font-semibold text-yellow-600">Sun Films</span>,
        <span class="font-semibold text-orange-500">Screen Guards</span>,
        <span class="font-semibold text-yellow-600"
          >PPF (Paint Protection Film)</span
        >, and
        <span class="font-semibold text-orange-500"
          >Nano Ceramic Safety Glazing Films</span
        >. They protect your vehicle, enhance comfort, and give it a lasting
        shine.
      </p>

      <p class="text-gray-700 text-base sm:text-lg leading-relaxed">
        We take pride in delivering
        <span class="font-semibold text-orange-500">exceptional products</span>
        while maintaining strong
        <span class="font-semibold text-yellow-500">customer satisfaction</span
        >. Our commitment to
        <span class="font-semibold text-orange-500"
          >quality, innovation, and service</span
        >
        sets us apart.
      </p>
    </div>
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

/* Mobile adjustments */
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

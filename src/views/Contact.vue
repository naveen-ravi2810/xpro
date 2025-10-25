<template>
  <section
    class="relative px-6 py-16 bg-gray-50 min-h-screen flex flex-col justify-between"
  >
    <!-- Header -->
    <div class="max-w-3xl mx-auto text-center mb-12">
      <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-4">
        Contact Us
      </h2>
      <p class="text-gray-700 text-base sm:text-lg">
        We're your trusted friends for automotive protection. Reach out and
        we'll assist you with our high-quality products.
      </p>
    </div>

    <!-- Contact Cards -->
    <div class="max-w-4xl mx-auto grid gap-8 sm:grid-cols-2 lg:grid-cols-3">
      <!-- Email Card -->
      <div
        class="flex flex-col items-center bg-white shadow-md rounded-xl p-6 hover:shadow-xl transition duration-300 text-center"
      >
        <!-- Email Icon -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-10 w-10 text-yellow-500 mb-4"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M16 12h2m4 0h-2m-4 0v2m0 4v-2M4 6h16M4 6v12h16V6M4 6l8 6 8-6"
          />
        </svg>
        <h3 class="text-xl font-semibold text-gray-900 mb-1">Email</h3>
        <a
          href="mailto:enquiries.xpro@gmail.com"
          class="text-gray-700 hover:text-yellow-600 font-medium text-sm sm:text-base"
        >
          enquiries.xpro@gmail.com
        </a>
      </div>

      <!-- Phone Card -->
      <div
        class="flex flex-col items-center bg-white shadow-md rounded-xl p-6 hover:shadow-xl transition duration-300 text-center"
      >
        <!-- Phone Icon -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-10 w-10 text-yellow-500 mb-4"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.518 4.555a1 1 0 01-.21 1.054l-2.083 2.083a16 16 0 006.83 6.83l2.083-2.083a1 1 0 011.054-.21l4.555 1.518a1 1 0 01.684.948V19a2 2 0 01-2 2h-1c-9.941 0-18-8.059-18-18V5z"
          />
        </svg>
        <h3 class="text-xl font-semibold text-gray-900 mb-1">Phone</h3>
        <div class="flex flex-col gap-1">
          <a
            href="tel:9962203441"
            class="text-gray-700 hover:text-yellow-600 font-medium text-sm sm:text-base"
            >9962203441</a
          >
          <a
            href="tel:7305333441"
            class="text-gray-700 hover:text-yellow-600 font-medium text-sm sm:text-base"
            >7305333441</a
          >
        </div>
      </div>

      <!-- Address Card -->
      <div
        class="flex flex-col items-center bg-white shadow-md rounded-xl p-6 hover:shadow-xl transition duration-300 text-center"
      >
        <!-- Location Icon -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-10 w-10 text-yellow-500 mb-4"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 11c1.104 0 2-.896 2-2s-.896-2-2-2-2 .896-2 2 .896 2 2 2z"
          />
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 22s8-4.5 8-10c0-4.418-3.582-8-8-8s-8 3.582-8 8c0 5.5 8 10 8 10z"
          />
        </svg>
        <h3 class="text-xl font-semibold text-gray-900 mb-1">Address</h3>
        <p class="text-gray-700 text-sm sm:text-base">
          130, Surya Narayana St, Kalmandapam, <br />
          Royapuram, Chennai, TN 600013
        </p>
      </div>
    </div>

    <!-- Footer -->
    <footer class="mt-16 text-center text-gray-500 text-sm">
      &copy; {{ new Date().getFullYear() }} X-Pro. All rights reserved.
    </footer>
  </section>
</template>

<script setup></script>

<style scoped>
/* Card hover lift effect */
div[class*="bg-white"]:hover {
  transform: translateY(-5px);
}

/* Smooth transition for hover effect */
div[class*="bg-white"] {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
</style>

<template>
  <header
    class="sticky top-0 left-0 w-full bg-white/80 backdrop-blur-md z-20 flex items-center justify-between px-6 py-3 shadow-md"
  >
    <div class="flex items-center space-x-3">
      <img
        src="@/assets/logo.png"
        alt="X-Pro Logo"
        class="w-10 h-10 sm:w-12 sm:h-12 object-contain"
      />
      <h2 class="text-xl sm:text-2xl font-bold text-gray-800 tracking-wide">
        X-Pro
      </h2>
    </div>
    <p class="hidden sm:block text-gray-500 text-sm">SunFlim & ScreenGuard</p>
  </header>
</template>

<style scoped>
@media (max-width: 640px) {
  header {
    padding: 0.5rem 1rem;
  }

  h2 {
    font-size: 1.25rem;
  }

  img {
    width: 36px;
    height: 36px;
  }

  p {
    font-size: 0.85rem;
  }
}
</style>

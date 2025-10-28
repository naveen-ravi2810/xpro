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
    <div class="flex items-center gap-3">
      <button @click="downloadBrochure" class="download-btn">
        Download Brochure
      </button>
      <p class="hidden sm:block text-gray-500 text-sm">SunFlim & ScreenGuard</p>
    </div>
  </header>
</template>
<script setup>
function downloadBrochure() {
  const pdfUrl = new URL("@/assets/Brochure.pdf", import.meta.url).href;

  // Create an anchor element and trigger the download
  const link = document.createElement("a");
  link.href = pdfUrl;
  link.download = "X-Pro-Brochure.pdf";
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}
</script>
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
.download-btn {
  background-color: #1c151d;
  color: white;
  border: none;
  padding: 10px 16px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 600;
}

.download-btn:hover {
  background-color: #0056b3;
}
</style>

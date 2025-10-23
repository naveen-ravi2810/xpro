<template>
  <section class="p-8">
    <h2 class="text-3xl font-semibold mb-4">Projects</h2>
    <ul class="space-y-4">
      <li
        v-for="(project, index) in projects"
        :key="index"
        class="border p-4 rounded"
      >
        <h3 class="font-bold text-xl">{{ project.name }}</h3>
        <p>{{ project.description }}</p>
      </li>
    </ul>
  </section>
</template>

<script setup>
const projects = [
  {
    name: "Agora Video App",
    description: "Real-time video conferencing using Vue and Django",
  },
  { name: "SpecBook", description: "PDF management and TOC parsing system" },
];
</script>

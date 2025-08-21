<template>
  <div class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gradient-to-br from-[#e0f2fe] to-[#f0e0ff] py-12 px-4 sm:px-6 lg:px-8">
    <!-- Decorative background shapes, similar to previous components -->
    <div class="absolute top-0 left-0 w-48 h-48 bg-blue-200 rounded-full mix-blend-multiply filter blur-xl opacity-30"></div>
    <div class="absolute bottom-0 right-0 w-64 h-64 bg-white rounded-full mix-blend-multiply filter blur-xl opacity-50"></div>

    <div class="relative z-10 w-full max-w-4xl mx-auto aspect-video bg-red-500 rounded-xl shadow-2xl overflow-hidden flex items-center justify-center">
      <!-- This is the "red section" where the image will be fitted -->
      <!-- Replace the placeholder.svg with your actual image URL -->
      <img
        src="/src/assets/Apple.png"
        alt="Content image for Streann Studio"
        class="w-full h-full object-cover"
      />
    </div>
  </div>
</template>

<script setup>
// No script logic needed for this static component
import Apple from '../assets/Apple.png'
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
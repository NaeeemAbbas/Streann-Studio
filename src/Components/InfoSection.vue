<template>
  <div class="relative min-h-screen flex items-center justify-center overflow-hidden  py-12 px-4 sm:px-6 lg:px-8">
    <!-- Decorative circles and spheres -->
    <div class="absolute top-1/2 left-1/4 w-32 h-32 bg-orange-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob"></div>
    <div class="absolute bottom-1/4 right-1/4 w-12 h-12 bg-white rounded-full shadow-lg"></div>

    <div class="relative z-10 max-w-7xl mx-auto text-center lg:text-left">
      <section class="flex flex-col lg:flex-row items-center justify-between gap-12 py-12">
        <div class="lg:w-1/2 space-y-6">
          <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
            Don't Put All Your Eggs In
            <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
              The Wrong Basket...
            </span>
          </h2>
          <p class="text-lg sm:text-xl text-gray-700">
            Think about it, what happens when the big content platforms don't like your content? They shut you down in two seconds. Even if it's a mistake.
          </p>
          <p class="text-lg sm:text-xl text-gray-700">
            Instead, with Streann Studio, there's no one to kick you out. No one to shadowban you. Because YOU are the one making the rules.
          </p>
        </div>
        <div class="lg:w-1/2 relative flex justify-center items-center">
          <img
            src="../assets/iMac 24 inch.png"
            alt="Streann Studio on Desktop"
            width="600"
            height="400"
            class="w-full h-auto object-contain"
          />
        </div>
      </section>
    </div>
  </div>
</template>

<script setup>
// No script logic needed for this static component
</script>

<style scoped>
/* Reusing the blob animation from previous components */
@keyframes blob {
  0% {
    transform: translate(0px, 0px) scale(1);
  }
  33% {
    transform: translate(30px, -50px) scale(1.1);
  }
  66% {
    transform: translate(-20px, 20px) scale(0.9);
  }
  100% {
    transform: translate(0px, 0px) scale(1);
  }
}

.animate-blob {
  animation: blob 7s infinite cubic-bezier(0.6, 0.01, 0.3, 0.9);
}
</style>
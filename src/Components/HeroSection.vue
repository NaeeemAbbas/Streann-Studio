<template>
  <div class="relative min-h-screen flex items-center justify-center overflow-hidden  py-12 px-4 sm:px-6 lg:px-8">
    <!-- Decorative circles -->
    <div class="absolute top-10 left-10 w-24 h-24  rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob"></div>
    <div class="absolute bottom-20 right-20 w-32 h-32 bg-blue-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-2000"></div>
    <div class="absolute top-1/4 right-1/4 w-20 h-20 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-4000"></div>

    <div class="relative z-10 max-w-7xl mx-auto text-center space-y-10">
      <h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-extrabold tracking-tight text-gray-900 leading-tight">
        With
        <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
          Streann Studio
        </span>
        You Can Make Content Creation, Monetization, And Distribution Effortless
      </h1>

      <div class="relative w-full max-w-5xl mx-auto overflow-hidden border border-gray-200">
        <img
          src="../assets/BCD_JBB0523-00708 2 (1).jpg"
          alt="Streann Studio Application Interface"
          width="900"
          height="500"
          class="w-full h-auto object-cover"
        />
      </div>

      <p class="mt-8 text-lg sm:text-xl text-gray-700 max-w-3xl mx-auto">
        This All-In-One Platform For Content Creators Will Save You Hours Of Work Per Week And Give You Full Control Over Your Business
      </p>

      <button class="mt-10 inline-flex cursor-pointer items-center justify-center px-8 py-4 border border-transparent text-base font-semibold rounded-xl shadow-lg text-white bg-gradient-to-r from-blue-500 to-purple-600 hover:from-blue-600 hover:to-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-all duration-300 ease-in-out transform hover:-translate-y-1">
        Get Started
      </button>
    </div>
  </div>
</template>

<script setup>
// No script logic needed for this static component
</script>

<style>
/* Tailwind CSS is automatically included.
   Custom animations for the blob effect. */
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

.animation-delay-2000 {
  animation-delay: 2s;
}

.animation-delay-4000 {
  animation-delay: 4s;
}
</style>
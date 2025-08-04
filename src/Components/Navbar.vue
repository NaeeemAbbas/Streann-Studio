<template>
  <header class="relative flex h-20 w-full items-center justify-between px-4 md:px-6 mx-auto max-w-6xl">
    <!-- Background gradient/pattern on the left -->
    <div class="absolute left-0 top-0 h-full w-1/3 bg-gradient-to-br from-[#e0f2fe] to-[#f0e0ff] opacity-50">
   
    </div>

    <!-- Logo -->
    <div class="relative z-10 flex items-center space-x-2">
      <img src="/src/assets/logo.png" alt="">
    </div>

    <!-- Desktop Navigation -->
    <nav class="hidden lg:flex items-center space-x-8 relative z-10">
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium">About us</a>
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium">FAQs</a>
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium">Portfolio</a>
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium">How it works</a>
      <button
      class="hidden lg:block relative z-10 px-6 py-3 rounded-lg text-white font-semibold
             bg-gradient-to-r from-blue-400 to-purple-500 hover:from-blue-500 hover:to-purple-600
             transition-all duration-200 shadow-lg cursor-pointer"
    >
      Get Started
    </button>
    </nav>

    <!-- Get Started Button (Desktop) -->
    

    <!-- Mobile Menu Button -->
    <button @click="toggleMobileMenu" class="lg:hidden relative z-10 p-2 rounded-md text-gray-700 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-blue-500">
      <svg
        class="h-6 w-6"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        ></path>
      </svg>
      <span class="sr-only">Open main menu</span>
    </button>

    <!-- Mobile Menu Overlay -->
    <transition name="slide-fade">
      <div
        v-if="isMobileMenuOpen"
        class="fixed inset-0 z-20 bg-[#fff] lg:hidden flex flex-col items-center justify-center space-y-6 p-4"
      >
        <button @click="toggleMobileMenu" class="absolute top-4 right-4 p-2 rounded-md text-gray-700 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-blue-500">
          <svg
            class="h-6 w-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M6 18L18 6M6 6l12 12"
            ></path>
          </svg>
          <span class="sr-only">Close main menu</span>
        </button>

        <a href="#" class="text-2xl text-gray-800 hover:text-blue-500 font-medium" @click="toggleMobileMenu">About us</a>
        <a href="#" class="text-2xl text-gray-800 hover:text-blue-500 font-medium" @click="toggleMobileMenu">FAQs</a>
        <a href="#" class="text-2xl text-gray-800 hover:text-blue-500 font-medium" @click="toggleMobileMenu">Portfolio</a>
        <a href="#" class="text-2xl text-gray-800 hover:text-blue-500 font-medium" @click="toggleMobileMenu">How it works</a>

        <button
          class="mt-8 px-8 py-4 rounded-lg text-white text-xl font-semibold
                 bg-gradient-to-r from-blue-400 to-purple-500 hover:from-blue-500 hover:to-purple-600
                 transition-all duration-200 shadow-lg"
          @click="toggleMobileMenu"
        >
          Get Started
        </button>
      </div>
    </transition>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const isMobileMenuOpen = ref(false);

const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};
</script>

<style scoped>
/* Transition styles for mobile menu */
.slide-fade-enter-active,
.slide-fade-leave-active {
  transition: all 0.3s ease-out;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(100%);
  opacity: 0;
}
</style>
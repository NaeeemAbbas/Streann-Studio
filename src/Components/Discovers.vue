<template>
  <div class="relative min-h-screen flex flex-col items-center justify-center overflow-hidden  py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto text-center space-y-10">
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
        Discover The True Power Of
        <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
          Content Monetization...
        </span>
      </h2>

      <p class="text-lg sm:text-xl text-gray-700 max-w-3xl mx-auto">
        With Streann Studio you have three major ways to monetize your content without showing annoying ads to your audience or chasing down sponsors.
      </p>

      <div class="mt-12 grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Card 1: Monthly Subscriptions -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border-t-4 border-b-4 border-transparent hover:border-cyan-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-300 to-cyan-500 flex items-center justify-center mb-4 shadow-md">
            <LayoutGridIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Monthly Subscriptions</h3>
          <p class="text-gray-700">
            Enjoy a solid recurring revenue stream by offering viewers paid subscriptions to access exclusive content.
          </p>
        </div>

        <!-- Card 2: PPV videos -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border-t-4 border-b-4 border-transparent hover:border-b-pink-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-pink-300 to-pink-500 flex items-center justify-center mb-4 shadow-md">
            <LockIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">PPV videos</h3>
          <p class="text-gray-700">
            Turn your best videos into gated content that raving fans will happily pay for.
          </p>
        </div>

        <!-- Card 3: 1-on-1 sessions -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border-t-4 border-b-4 border-transparent hover:border-orange-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-orange-300 to-orange-500 flex items-center justify-center mb-4 shadow-md">
            <UserIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">1-on-1 sessions</h3>
          <p class="text-gray-700">
            This is your chance to connect with your audience in a more personalized setting, for a higher fee.
          </p>
        </div>
      </div>

      <p class="mt-10 text-lg sm:text-xl text-gray-700 max-w-3xl mx-auto">
        Plus, you can also accept viewer donations if you prefer. Which means you have a multitude of ways to grow your business and make money.
      </p>
    </div>
  </div>
</template>

<script setup>
import { LayoutGridIcon, LockIcon, UserIcon } from 'lucide-vue-next';
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
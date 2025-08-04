<template>
  <div class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gradient-to-br from-[#e0f2fe] to-[#f0e0ff] py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto text-center space-y-10">
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
        Don't Take Our Word For It... See Why Others Are
        <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
          Loving Streann Studio
        </span>
      </h2>

      <div class="mt-12 grid grid-cols-1 lg:grid-cols-2 gap-8 items-start">
        <!-- Large Testimonial Card -->
        <div class="bg-white rounded-xl shadow-lg p-6 border cursor-pointer border-blue-100 flex flex-col justify-between h-full">
          <p class="text-gray-700 text-left mb-6 text-lg">
            "This is just awesome! I am so impressed with not only the amazing product, but the outstanding customer service! If you are looking for a streaming product with the personal approach then this is the one! I cannot recommend this enough!"
          </p>
          <div class="flex items-center justify-between mt-auto">
            <div class="flex items-center">
              <UserIcon class="w-6 h-6 text-blue-500 mr-2" />
              <span class="font-semibold text-gray-800">Justine</span>
            </div>
            <div class="flex">
              <StarIcon v-for="i in 5" :key="i" class="w-5 h-5 text-orange-400 fill-current" />
            </div>
          </div>
        </div>

        <!-- Stacked Small Testimonial Cards -->
        <div class="grid grid-cols-1 gap-8">
          <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border border-blue-100 flex flex-col justify-between">
            <p class="text-gray-700 text-left mb-4">
              "It's like Canva for Streaming!"
            </p>
            <div class="flex items-center justify-between mt-auto">
              <div class="flex items-center">
                <UserIcon class="w-6 h-6 text-blue-500 mr-2" />
                <span class="font-semibold text-gray-800">Tala</span>
              </div>
              <div class="flex">
                <StarIcon v-for="i in 5" :key="i" class="w-5 h-5 text-orange-400 fill-current" />
              </div>
            </div>
          </div>

          <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border border-blue-100 flex flex-col justify-between">
            <p class="text-gray-700 text-left mb-4">
              "It is the easiest choice of all. It is pretty awesome!"
            </p>
            <div class="flex items-center justify-between mt-auto">
              <div class="flex items-center">
                <UserIcon class="w-6 h-6 text-blue-500 mr-2" />
                <span class="font-semibold text-gray-800">Chris</span>
              </div>
              <div class="flex">
                <StarIcon v-for="i in 5" :key="i" class="w-5 h-5 text-orange-400 fill-current" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { UserIcon, StarIcon } from 'lucide-vue-next';
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
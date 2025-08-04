<template>
  <div class="relative min-h-screen flex items-center justify-center overflow-hidden  py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto text-center space-y-10">
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
        Want To Become
        <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
          The #1 Content Creator
        </span>
        In Your Industry? Here Are 3 Steps...
      </h2>

      <div class="mt-12 grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Card 1: Get Started Today -->
        <div class="bg-white rounded-xl h-96 cursor-pointer shadow-lg p-6 border-t-4 border-b-4 border-transparent hover:border-orange-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-orange-300 to-orange-500 flex items-center justify-center mb-4 shadow-md">
            <ThumbsUpIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Get Started Today</h3>
          <p class="text-gray-700">
            Start using Streann Studio today and see how easy and rewarding it becomes to create high-value, money-making content.
          </p>
        </div>

        <!-- Card 2: Create More Strategic Content -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border-t-4 border-b-4 border-transparent hover:border-cyan-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-300 to-cyan-500 flex items-center justify-center mb-4 shadow-md">
            <RocketIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Create More Strategic Content</h3>
          <p class="text-gray-700">
            When you use Streann Studio you'll be able to create only top-notch content. Which means more viewers, more subscribers, and more fame.
          </p>
        </div>

        <!-- Card 3: Run A Real Business -->
        <div class="bg-white rounded-xl shadow-lg cursor-pointer p-6 border-t-4 border-b-4 border-transparent hover:border-purple-400 transition-all duration-300 ease-in-out flex flex-col items-center text-center">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-purple-300 to-purple-500 flex items-center justify-center mb-4 shadow-md">
            <ShoppingBagIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Run A Real Business</h3>
          <p class="text-700">
            Instead of chasing sponsors or showing annoying ads, Streann Studio gives you all the monetization strategies and subscriber data tools you need to run a real business as a content creator.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ThumbsUpIcon, RocketIcon, ShoppingBagIcon } from 'lucide-vue-next';
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
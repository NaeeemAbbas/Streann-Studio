<template>
  <div class="relative min-h-screen flex flex-col items-center justify-center overflow-hidden  py-12 px-4 sm:px-6 lg:px-8">
    <!-- Decorative circles and spheres for the top section -->
    <div class="absolute top-10 right-1/4 w-24 h-24  rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob"></div>
    <div class="absolute top-1/3 left-1/4 w-16 h-16  rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-2000"></div>
    <div class="absolute top-[40%] left-[30%] w-10 h-10 bg-white rounded-full shadow-lg"></div>

    <div class="relative z-10 max-w-7xl mx-auto text-center lg:text-left space-y-20">
      <!-- Top Section: All-in-One Platform -->
      <section class="flex flex-col lg:flex-row items-center justify-between gap-12 py-12">
        <div class="lg:w-1/2 space-y-6">
          <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
            More Than Streaming: This Is Your
            <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text  decoration-blue-500 decoration-wavy">
              All-In-One Platform For Explosive Growth & Profits
            </span>
          </h2>
          <p class="text-lg sm:text-xl text-gray-700">
            Stop relying on third-party platforms with their algorithms and sudden policy changes. If you want to be in full control of your business as a content creator... if you want to create your own platform where YOU make the rules...
          </p>
          <p class="text-lg sm:text-xl text-gray-700 font-semibold">
            Then try Streann Studio today.
          </p>
        </div>
        <div class="lg:w-1/2 relative flex justify-center items-center">
          <img
            :src="Apple"
            alt="Streann Studio on Desktop and Tablet"
            width="600"
            height="400"
            class="w-full h-auto object-contain"
          />
        </div>
      </section>

      <!-- Decorative circles and spheres for the bottom section -->
      <div class="absolute bottom-10 left-1/4 w-24 h-24 bg-pink-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-4000"></div>
      <div class="absolute bottom-1/3 right-1/4 w-16 h-16 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-6000"></div>
      <div class="absolute bottom-[40%] right-[30%] w-10 h-10 bg-white rounded-full shadow-lg"></div>

      <!-- Bottom Section: 60,000 Content Creators -->
      <section class="flex flex-col lg:flex-row-reverse items-center justify-between gap-12 py-12">
        <div class="lg:w-1/2 space-y-6 lg:text-left text-center">
          <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
            There's A Reason Why Over 60,000 Content Creators Use
            <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
              Streann Studio...
            </span>
          </h2>
          <p class="text-lg sm:text-xl text-gray-700">
            Imagine you could turn your love for high-quality content creation into an actual business... without having to beg sponsors for deals.
          </p>
          <p class="text-lg sm:text-xl text-gray-700">
            Imagine being able to monetize your content without compromising your values and showing your viewers annoying ads all the time.
          </p>
          <p class="text-lg sm:text-xl text-gray-700">
            This is what's possible when you have a channel that's engineered to make content monetization simple and easy.
          </p>
        </div>
        <div class="lg:w-1/2 relative flex justify-center items-center">
          <img
            :src="Group"
            alt="Streann Studio on Laptop"
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
import Apple from  '../assets/Apple.png';
import  Group from '../assets/Group.png';
</script>

<style scoped>
/* Reusing the blob animation from the first component */
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

.animation-delay-6000 {
  animation-delay: 6s;
}
</style>
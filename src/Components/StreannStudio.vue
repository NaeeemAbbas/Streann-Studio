<template>
  <div class="relative min-h-screen flex flex-col items-center justify-center overflow-hidden py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto text-center space-y-10">
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
        Here's Just A Taste Of What
        <span class="bg-gradient-to-r from-blue-500 to-cyan-400 text-transparent bg-clip-text">
          Streann Studio
        </span>
        Can Do For You...
      </h2>

      <div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Feature Card 1 -->
        <div class="bg-white rounded-xl shadow-lg p-6 cursor-pointer border border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-300 to-cyan-500 flex items-center justify-center mb-4 shadow-md">
            <DollarSignIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Monetize Your Content On Your Own Terms</h3>
          <p class="text-gray-700">
            No more annoying your audience with interrupting ads (whether it's sponsored content or an actual ad from the platform). Instead, you'll have several ways to monetize your work without appearing sleazy.
          </p>
        </div>

        <!-- Feature Card 2 -->
        <div class="bg-white rounded-xl shadow-lg p-6 cursor-pointer border border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-orange-300 to-orange-500 flex items-center justify-center mb-4 shadow-md">
            <DatabaseIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Own 100% Of Your Data</h3>
          <p class="text-gray-700">
            Instead of keeping your subscribers hostage like major platforms, we give them all to you. You own your subscriber data so you know that, no matter what happens, your hard work won't go to waste.
          </p>
        </div>

        <!-- Feature Card 3 -->
        <div class="bg-white rounded-xl shadow-lg p-6 border cursor-pointer border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-orange-300 to-orange-500 flex items-center justify-center mb-4 shadow-md">
            <MonitorIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Grow Your Brand Across All Platforms</h3>
          <p class="text-gray-700">
            Amplify your brand and your impact all over your favorite social media channels like Facebook, YouTube, Twitch, LinkedIn, and more... by going live in all of them at the same time!
          </p>
        </div>

        <!-- Feature Card 4 -->
        <div class="bg-white rounded-xl  cursor-pointer shadow-lg p-6 border border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-pink-300 to-pink-500 flex items-center justify-center mb-4 shadow-md">
            <UsersIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Invite Guests To Your Streams With Zero Headaches</h3>
          <p class="text-gray-700">
            If you want to share the stage and collaborate with others, you can use Streann Studio to set up everything in just a few seconds. No matter what software or device your guests are using.
          </p>
        </div>

        <!-- Feature Card 5 -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-pink-300 to-pink-500 flex items-center justify-center mb-4 shadow-md">
            <ImagePlusIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Attention-Grabbing Banners</h3>
          <p class="text-gray-700">
            Include banners in real-time to your live streams to keep people's attention and skyrocket your engagement.
          </p>
        </div>

        <!-- Feature Card 6 -->
        <div class="bg-white rounded-xl cursor-pointer shadow-lg p-6 border border-blue-100 flex flex-col items-start text-left">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-300 to-cyan-500 flex items-center justify-center mb-4 shadow-md">
            <PlayIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Go Live With Pre-Recorded Shows</h3>
          <p class="text-gray-700">
            Imagine grabbing all of your previous, highly-successful streams... the ones that got you hundreds of subscribers and that your people LOVED... and reusing them as "lives" when you want a boost in subscribers and engagement. You can easily do it with Streann Studio!
          </p>
        </div>

        <!-- Feature Card 7 (Spans full width on mobile, half on desktop) -->
        <div class="bg-white cursor-pointer rounded-xl shadow-lg p-6 border border-blue-100 flex flex-col items-start text-left md:col-span-1">
          <div class="w-16 h-16 rounded-full bg-gradient-to-br from-cyan-300 to-cyan-500 flex items-center justify-center mb-4 shadow-md">
            <MessageSquareIcon class="w-8 h-8 text-white" />
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Chat with Guests & Privately Share Your Screen</h3>
          <p class="text-gray-700">
            Want to make sure every time you invite a guest things go smoothly and perfectly? With private chat and private screen sharing you can coordinate with guests on the fly to make sure everything works out just like you want to!
          </p>
        </div>

        <!-- Get Started Button (Aligned to the right, next to the last card on desktop) -->
        <div class="flex items-end justify-center md:justify-end md:col-span-1">
          <button class="inline-flex items-center cursor-pointer justify-center px-8 py-4 border border-transparent text-base font-semibold rounded-lg shadow-lg text-white bg-gradient-to-r from-blue-500 to-purple-600 hover:from-blue-600 hover:to-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-all duration-300 ease-in-out transform hover:-translate-y-1">
            Get Started
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { DollarSignIcon, DatabaseIcon, MonitorIcon, UsersIcon, ImagePlusIcon, PlayIcon, MessageSquareIcon } from 'lucide-vue-next';
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
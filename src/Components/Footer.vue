<template>
  <footer class="relative overflow-hidden bg-gradient-to-br   py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-8 text-gray-700">
      <!-- Logo and Tagline Section -->
      <div class="flex flex-col items-center md:items-start text-center md:text-left space-y-4">
        <div class="flex items-center space-x-2">
          <img
            src="/src/assets/logo.png"
            alt="Streann Studio Logo"
            width="40"
            height="40"
            class="h-10 w-full"
          />
          
        </div>
        <p class="text-lg">Empower your business with live streaming!</p>
      </div>

      <!-- Contact Info Section -->
      <div class="space-y-4 text-center md:text-left">
        <h3 class="text-xl font-bold text-gray-900 mb-2">Contact Info</h3>
        <div class="flex items-center justify-center md:justify-start space-x-3">
          <div class="w-8 h-8 rounded-full bg-cyan-300 flex items-center justify-center shadow-sm">
            <MapPinIcon class="w-4 h-4 text-white" />
          </div>
          <span>7791 NW 48 Street, Suite 324. Miami Fl 33166</span>
        </div>
        <div class="flex items-center justify-center md:justify-start space-x-3">
          <div class="w-8 h-8 rounded-full bg-pink-300 flex items-center justify-center shadow-sm">
            <PhoneIcon class="w-4 h-4 text-white" />
          </div>
          <span>1-888-70-ON-AIR (66247)</span>
        </div>
        <div class="flex items-center justify-center md:justify-start space-x-3">
          <div class="w-8 h-8 rounded-full bg-orange-300 flex items-center justify-center shadow-sm">
            <MailIcon class="w-4 h-4 text-white" />
          </div>
          <div>
            <span>studio@streann.com</span>
            <a href="#" class="block text-blue-600 hover:underline">Partner Program</a>
          </div>
        </div>
      </div>

      <!-- Legal Links and Social Media -->
      <div class="space-y-6 text-center md:text-left">
        <div class="flex justify-center md:justify-start space-x-4">
          <button class="px-4 py-2 rounded-full border border-gray-300 text-gray-700 hover:bg-gray-100 transition-colors">Privacy Policy</button>
          <button class="px-4 py-2 rounded-full border border-gray-300 text-gray-700 hover:bg-gray-100 transition-colors">Terms of use</button>
        </div>
        <div class="flex justify-center md:justify-start space-x-4">
          <a href="#" aria-label="Twitter" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <TwitterIcon class="w-5 h-5 text-white" />
          </a>
          <a href="#" aria-label="Facebook" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <FacebookIcon class="w-5 h-5 text-white" />
          </a>
          <a href="#" aria-label="Instagram" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <InstagramIcon class="w-5 h-5 text-white" />
          </a>
          <a href="#" aria-label="LinkedIn" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <LinkedinIcon class="w-5 h-5 text-white" />
          </a>
          <a href="#" aria-label="TikTok" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <TikTokIcon class="w-5 h-5 text-white" />
          </a>
        </div>
      </div>

      <!-- Partner Program and Robot Icon -->
      <div class="flex flex-col items-center md:items-start text-center md:text-left space-y-4 lg:col-span-1">
        <h3 class="text-xl font-bold text-gray-900 mb-2">Partner Program</h3>
        <img
          src="/src/assets/FooterImg.png"
          alt="Chatbot icon"
          width="80"
          height="80"
          class="mt-auto"
        />
      </div>
    </div>

    <!-- Copyright Section -->
    <div class="mt-12 pt-8 border-t border-gray-200 text-center text-gray-600 text-sm">
      © 2023 Streann Media. All rights reserved
    </div>
  </footer>
</template>

<script setup>
import { MapPinIcon, PhoneIcon, MailIcon, TwitterIcon, FacebookIcon, InstagramIcon, LinkedinIcon } from 'lucide-vue-next';

// Custom TikTok icon as it's not directly in lucide-vue-next
const TikTokIcon = {
  props: {
    class: String
  },
  template: `
    <svg :class="class" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
      <path d="M12.525 1.151c-1.416-1.397-3.942 0-3.942 0v4.701c-4.048 1.18-8.064 5.198-8.064 9.205 0 5.04 4.06 9.101 9.101 9.101 5.04 0 9.101-4.06 9.101-9.101 0-3.942-2.53-7.959-6.578-9.138V1.151zM17.5 14.5c0 2.76-2.24 5-5 5s-5-2.24-5-5 2.24-5 5-5 5 2.24 5 5z"/>
    </svg>
  `
};
</script>

<style scoped>
/* No specific styles needed beyond Tailwind classes */
</style>
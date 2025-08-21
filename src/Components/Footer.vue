<template>
  <footer class="relative overflow-hidden bg-gradient-to-br   py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative z-10 max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-8 text-gray-700">
      <!-- Logo and Tagline Section -->
      <div class="flex flex-col items-center md:items-start text-center md:text-left space-y-4">
        <div class="flex items-center space-x-2">
          <img
            :src="logo"
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
          <a href="#" aria-label="Github" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-gray-700 transition-colors">
            <Github class="w-5 h-5 text-white" />
          </a>
        </div>
      </div>

      <!-- Partner Program and Robot Icon -->
      <div class="flex flex-col items-center md:items-start text-center md:text-left space-y-4 lg:col-span-1">
        <h3 class="text-xl font-bold text-gray-900 mb-2">Partner Program</h3>
        <img
          :src="FooterImg"
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
import logo from '../assets/Logo.png'
import FooterImg from '../assets/FooterImg.png'

import { MapPinIcon, PhoneIcon, MailIcon, TwitterIcon, FacebookIcon, InstagramIcon, LinkedinIcon, TicketCheckIcon, Github } from 'lucide-vue-next';

// Custom TikTok icon as it's not directly in lucide-vue-next

</script>

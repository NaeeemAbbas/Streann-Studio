<template>
  <div class="relative min-h-screen flex flex-col items-center justify-center overflow-hidden py-12 px-4 sm:px-6 lg:px-8">
    <!-- Decorative circles -->
    <div class="absolute top-10 left-10 w-24 h-24 bg-pink-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob"></div>
    <div class="absolute bottom-20 right-20 w-32 h-32 bg-orange-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-2000"></div>
    <div class="absolute top-1/4 right-1/4 w-20 h-20 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-4000"></div>

    <div class="relative z-10 max-w-4xl mx-auto text-center space-y-10">
      <h2 class="text-3xl sm:text-4xl md:text-5xl font-extrabold tracking-tight text-gray-900 leading-tight">
        Frequently Asked Questions
      </h2>

      <div class="mt-12 w-full space-y-4">
        <div
          v-for="(faq, index) in faqs"
          :key="index"
          class="bg-white rounded-xl shadow-lg border border-blue-100 overflow-hidden transition-all duration-300"
        >
          <button
            @click="toggleFaq(index)"
            class="w-full flex justify-between items-center p-6 text-lg font-semibold text-gray-900 focus:outline-none"
            :class="{ 'text-blue-600': openIndex === index }"
          >
            <span>{{ faq.question }}</span>
            <ChevronUpIcon
              v-if="openIndex === index"
              class="w-6 h-6 text-blue-600 transform transition-transform duration-300 rotate-180"
            />
            <ChevronDownIcon
              v-else
              class="w-6 h-6 text-gray-500 transform transition-transform duration-300"
            />
          </button>

          <!-- Expandable content with fixed height and scroll -->
          <div
            class="transition-all duration-300 ease-in-out"
            :class="openIndex === index ? 'max-h-40 px-6 pb-4 overflow-y-auto' : 'max-h-0 px-6 pb-0 overflow-hidden'"
          >
            <p
              v-for="(paragraph, pIndex) in faq.answer"
              :key="pIndex"
              class="mb-2 text-left text-gray-700 last:mb-0"
            >
              <span
                v-if="faq.question === 'Can I try Streann Studio For Free?'"
                class="text-pink-500 mr-2"
              >
                •
              </span>
              {{ paragraph }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { ChevronUpIcon, ChevronDownIcon } from 'lucide-vue-next'

const openIndex = ref(null)

const faqs = ref([
  {
    question: 'Can I try Streann Studio For Free?',
    answer: [
      'Of course! You can sign up for a free account today by clicking the button below.',
      'However, if you already decided you want Streann Studio is for you and you want all the features, click here to check out our paid plans.'
    ]
  },
  {
    question: 'What platforms can I stream to using Streann Studio?',
    answer: [
      'Streann Studio supports streaming to multiple platforms simultaneously, including YouTube, Facebook, Twitch, LinkedIn, and more. You can reach your audience wherever they are.'
    ]
  },
  {
    question: 'Does Streann Studio provide analytics and insights on audience engagement?',
    answer: [
      'Yes, Streann Studio offers comprehensive analytics and insights into your audience engagement, subscriber data, and monetization performance to help you grow your business.'
    ]
  },
  {
    question: 'How many trailers can I buy?',
    answer: [
      'The number of trailers you can buy depends on your subscription plan. Please refer to our pricing page for detailed information on what each plan includes.'
    ]
  },
  {
    question: 'Is there a mobile app available for managing and accessing My Channel on the go?',
    answer: [
      'Yes, Streann Studio offers a mobile application for both iOS and Android devices, allowing you to manage your channel, stream, and interact with your audience from anywhere.'
    ]
  }
])

const toggleFaq = (index) => {
  openIndex.value = openIndex.value === index ? null : index
}
</script>

<style scoped>
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

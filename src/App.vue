<script setup>
import About from './Components/About.vue';
import ContentCreator from './Components/ContentCreator.vue';
import Discovers from './Components/Discovers.vue';
import Faqs from './Components/Faqs.vue';
import Footer from './Components/Footer.vue';
import HeroSection from './Components/HeroSection.vue';
import ImageComponent from './Components/ImageComponent.vue';
import InfoSection from './Components/InfoSection.vue';
import Navbar from './Components/Navbar.vue';
import Rating from './Components/Rating.vue';
import StreannStudio from './Components/StreannStudio.vue';

</script>
<template>
  <div class="flex flex-col bg-gradient-to-br from-[#e0f2fe] to-[#f0e0ff]">
<Navbar/>
<HeroSection/>
  <ContentCreator/>
  <Rating/>
  <About/>
  <StreannStudio/>
  <InfoSection/>
  <Discovers/>
  <ImageComponent/>
  <Faqs/>
  <Footer/>
  </div>
</template>
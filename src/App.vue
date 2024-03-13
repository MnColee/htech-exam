<template>
  <header class="absolute top-0 inset-x-0 flex items-center justify-center w-full h-auto text-white z-50">
    <nav class="container w-full flex items-center justify-between border-b border-white p-4">
      <div class="logo w-1/4 flex items-center justify-start">
        <p class="font-bold text-green-400 text-2xl">Travel<span class="text-white">Blog</span></p>
      </div>
      
      <ul class="items-center justify-between w-3/6 font-base hidden md:flex">
        <li>Home</li>
        <li class="flex items-center gap-x-1.5">About Me<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Category<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Blog<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Contact Me<i class="fa-solid fa-chevron-down text-xs"></i></li>
      </ul>

      <div class="flex items-center justify-end gap-x-4 w-1/4">
        <i class="fa-brands fa-facebook-f hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i>
        <i class="fa-brands fa-twitter hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i>
        <i class="fa-brands fa-instagram hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i>
      </div>
    </nav>
  </header>
  
  <main class="flex align-middle justify-center h-auto flex-col">
    <HomeView />
    <CategorySection />
    <FeaturedExplore />
    <VideoSection />
    <Footer />
  </main>
</template>


<script setup>
import HomeView from './views/HomeView.vue';
import CategorySection from './views/CategorySection.vue'
import FeaturedExplore from './views/FeaturedExplore.vue';
import VideoSection from './views/VideoSection.vue';
import Footer from './views/Footer.vue';
</script>
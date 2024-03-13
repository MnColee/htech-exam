<template>
  <header class="absolute top-0 inset-x-0 flex items-center justify-center w-full h-auto text-white z-50">
    <nav class="container w-full flex flex-col items-center justify-between border-b border-white lg:flex-row">
      <div class="logo w-full flex items-center justify-between p-4 lg:justify-start lg:w-1/4">
        <p class="font-bold text-green-400 text-2xl">Travel<span class="text-white">Blog</span></p>
        <button type="button" @click="toggleMenu" class="text-white lg:hidden"><i class="fa-solid fa-bars"></i></button>
      </div>
      
      <ul :class="{ 'mobile-menu': true, 'open': menu }" class="menu flex-col gap-y-3 items-start justify-between w-full font-base p-4 lg:w-3/6 lg:flex lg:flex-row">
        <li>Home</li>
        <li class="flex items-center gap-x-1.5">About Me<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Category<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Blog<i class="fa-solid fa-chevron-down text-xs"></i></li>
        <li class="flex items-center gap-x-1.5">Contact Me<i class="fa-solid fa-chevron-down text-xs"></i></li>

        <div class="flex items-center justify-start gap-x-4 w-full mt-3 lg:hidden">
          <a href="#"><i class="fa-brands fa-facebook-f hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
          <a href="#"><i class="fa-brands fa-twitter hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
          <a href="#"><i class="fa-brands fa-instagram hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
        </div>
      </ul>

      <div class="hidden items-center justify-end gap-x-4 w-1/4 lg:flex lg:px-4">
        <a href="#"><i class="fa-brands fa-facebook-f hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
        <a href="#"><i class="fa-brands fa-twitter hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
        <a href="#"><i class="fa-brands fa-instagram hover:bg-orange-400 hover:text-white bg-white text-gray-500 rounded-full px-2.5 py-1.5 text-xs"></i></a>
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
import { ref } from 'vue';

const menu = ref(false);

const toggleMenu = ()=> {
  menu.value = !menu.value;
}
</script>

<style scoped>
.menu {
  background-color: #323232;
}

.mobile-menu {
    display: none;
    transition: width 0.3s ease;
}

.mobile-menu.open {
    display: flex;
}

@media only screen and (min-width: 1024px) {
    .menu {
      background-color: transparent;
    }

    .mobile-menu {
      display: flex;
    }
}
</style>
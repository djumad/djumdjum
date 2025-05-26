<template>
  <header>
    <nav :class="['fixed w-full z-50 transition-colors duration-300', isScrolled ? 'bg-white shadow-md text-gray-900' : 'bg-gradient-to-r from-blue-600 to-purple-600 text-white']">
      <div class="container mx-auto px-6 py-5 flex justify-between items-center">
        <div class="text-3xl font-extrabold tracking-wide">
          <span :class="isScrolled ? 'text-yellow-500' : 'text-yellow-300'">Porto</span><span>folio</span>
        </div>
        <ul class="hidden md:flex space-x-8 text-lg font-semibold">
          <li><a href="#about" class="hover:text-yellow-400 transition duration-300">Tentang</a></li>
          <li><a href="#projects" class="hover:text-yellow-400 transition duration-300">Proyek</a></li>
          <li><a href="#skills" class="hover:text-yellow-400 transition duration-300">Keterampilan</a></li>
          <li><a href="#contact" class="hover:text-yellow-400 transition duration-300">Kontak</a></li>
        </ul>
        <button class="md:hidden text-inherit focus:outline-none">
          <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </nav>

    <div class="pt-28 pb-32 bg-gradient-to-r from-blue-600 to-purple-600 text-white text-center animate-fade-in-up">
      <div class="container mx-auto px-6 h-100">
        <h1 class="text-5xl sm:text-6xl md:text-7xl font-extrabold leading-tight mb-8">
          Hai, Saya <span class="text-yellow-300">Djumad Bantan</span>
        </h1>
        <p class="text-xl sm:text-2xl md:text-3xl mb-10 opacity-90">
          Fullstack Developer Laravel + Vue 
        </p>
        <a href="#contact"
           class="bg-yellow-400 hover:bg-yellow-300 text-gray-900 px-10 py-4 rounded-full text-xl font-bold shadow-xl transition duration-300">
          Hubungi Saya
        </a>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})
onBeforeUnmount(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
@keyframes fadeInUp {
  0% {
    opacity: 0;
    transform: translateY(40px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in-up {
  animation: fadeInUp 1s ease-out forwards;
}
</style>

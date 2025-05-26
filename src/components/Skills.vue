<template>
  <section class="py-16">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-4">
        Keterampilan <span class="text-blue-600">Saya</span>
      </h2>
      <p class="text-center text-gray-600 mb-12 max-w-2xl mx-auto">
        Teknologi dan alat yang saya kuasai
      </p>

      <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-8">
        <div
          v-for="(skill, index) in skills"
          :key="index"
          class="flex flex-col items-center p-4 hover:bg-gray-100 rounded-lg transition"
        >
          <div class="w-16 h-16 mb-4">
            <img :src="skill.icon" :alt="skill.name" class="w-full h-full object-contain" />
          </div>
          <span class="font-medium">{{ skill.name }}</span>
          <div class="w-full bg-gray-200 rounded-full h-2 mt-2">
            <div class="bg-blue-600 h-2 rounded-full" :style="{ width: skill.level + '%' }"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import vueIcon from '../assets/vue-icon.png'
import jsIcon from '../assets/js-icon.png'
import tailwindIcon from '../assets/tailwind-icon.png'
import htmlIcon from '../assets/html-icon.png'
import cssIcon from '../assets/css-icon.png'
import gitIcon from '../assets/git-icon.png'
import nodeIcon from '../assets/node-icon.png'
import reactIcon from '../assets/react-icon.webp'
import laravelIcon from '../assets/laravel-icon.png'
import phpIcon from '../assets/php-icon.svg'
import tsIcon from '../assets/ts-icon.png'
import livewireIcon from '../assets/livewire-icon.svg'
import jquery from '../assets/jquery-icon.png'

const skills = [
  { name: 'Vue.js', icon: vueIcon, level: 90 },
  { name: 'JavaScript', icon: jsIcon, level: 85 },
  { name: 'Tailwind CSS', icon: tailwindIcon, level: 80 },
  { name: 'HTML5', icon: htmlIcon, level: 95 },
  { name: 'CSS3', icon: cssIcon, level: 85 },
  { name: 'Git', icon: gitIcon, level: 75 },
  { name: 'Node.js', icon: nodeIcon, level: 70 },
  { name: 'React', icon: reactIcon, level: 60 },
  { name: 'Laravel', icon: laravelIcon, level: 90 },
  { name: 'Php', icon: phpIcon, level: 65 },
  { name: 'TypeScript', icon: tsIcon, level: 60 },
  { name: 'Livewire', icon: livewireIcon, level: 70 },
  { name: 'Jquery', icon: jquery, level: 70 }
]
</script>

<template>
  <section class="py-16 bg-gray-100">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-4">Proyek <span class="text-purple-600">Saya</span></h2>
      <p class="text-center text-gray-600 mb-12 max-w-2xl mx-auto">
        Berikut beberapa proyek terbaru yang telah saya kerjakan
      </p>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-xl transition"
        >
          <div class="h-48 overflow-hidden">
            <img :src="project.image" :alt="project.title" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold mb-2">{{ project.title }}</h3>
            <p class="text-gray-600 mb-4">{{ project.description }}</p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span
                v-for="(tech, i) in project.technologies"
                :key="i"
                class="bg-gray-200 px-2 py-1 text-xs rounded"
              >
                {{ tech }}
              </span>
            </div>
            <a :href="project.link" target="_blank" class="text-purple-600 hover:text-purple-800 font-medium">
              Lihat Proyek →
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import project1 from '../assets/project1.png'
import project2 from '../assets/project2.png'
import project3 from '../assets/baguala.png'

const projects = [
  {
    title: 'Sistem Informasi Astekindo Maluku',
    description: 'Aplikasi Sistem Informasi LSP Astekindo Maluku menggunakan',
    technologies: ['Vue.js', 'Tailwind CSS', 'Pocketbase'],
    image: project1,
    link: 'https://astekindomaluku.vercel.app'
  },
  {
    title: 'Sistem Informasi Negeri Kaibobo',
    description: 'Aplikasi Sistem Informasi Negeri Kaibobo dengan menggunakan laravel, filament dan livewire',
    technologies: ['laravel', 'bootstrap', 'livewire' , 'jquery' , 'filament'],
    image: project2,
    link: 'https://negerikaibobo.id/'
  },
  {
    title: 'Baguala Techno',
    description: 'Website Company Profile Baguala Techno',
    technologies: ['livewire', 'Tailwind CSS' , 'laravel'],
    image: project3,
    link: 'https://bagualatechno.com/'
  }
]
</script>
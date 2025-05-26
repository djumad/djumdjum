<template>
  <div class="min-h-screen bg-gray-50">
    <Header />
    
    <main class="container mx-auto px-4 py-8">
      <About id="about" />
      <Projects id="projects" />
      <Skills id="skills" />
      <Contact id="contact" />
    </main>
    
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>
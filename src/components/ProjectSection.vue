<template>
  <section id="projects" class="relative bg-gradient-to-b from-[#0b1e26] to-[#12141a] text-white py-24 font-sarpanch">
    <!-- Top-left logo -->
    <img :src="HexLogo" alt="Logo Cluster" class="absolute top-6 left-6 z-20 w-12 h-12 object-contain" />


    <div class="relative z-10 max-w-screen-xl mx-auto px-6 text-center">
      <h2 class="text-4xl font-bold mb-2">Projects</h2>
      <p class="text-gray-300 mb-12">Press the figures to gain more information</p>

      <!-- Project Grid -->
      <div class="grid grid-cols-2 md:grid-cols-3 gap-6 place-items-center">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="w-[180px] h-[200px] relative cursor-pointer group"
          @click="openProject(index)"
        >
          <div class="absolute inset-0 border-4 border-purple-500 hex-border z-10 group-hover:border-cyan-400 transition duration-200"></div>
          <img
            :src="project.image"
            alt="Project image"
            class="w-full h-full object-cover hex-clip relative z-0"
          />
        </div>
      </div>
    </div>

    <!-- Project Modal -->
    <div v-if="activeProject !== null" class="fixed inset-0 z-50 bg-black bg-opacity-80 flex items-center justify-center px-4">
      <div class="bg-[#2e2f33] rounded-lg p-6 max-w-3xl w-full relative">
        <button @click="closeModal" class="absolute top-3 right-4 text-white text-3xl font-bold">&times;</button>
        <h3 class="text-2xl font-bold mb-4">{{ projects[activeProject].title }}</h3>
        <img :src="projects[activeProject].image" class="w-full max-h-64 object-cover mb-4 rounded-md" />
        <p class="text-gray-300">{{ projects[activeProject].description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import HexLogo from '@/assets/images/hex-two.png'

// Replace these with your real content later
const projects = ref([
  {
    title: 'Project A',
    image: 'https://via.placeholder.com/200x200?text=A',
    description: 'Description for Project A.',
  },
  {
    title: 'Project B',
    image: 'https://via.placeholder.com/200x200?text=B',
    description: 'Description for Project B.',
  },
  {
    title: 'Project C',
    image: 'https://via.placeholder.com/200x200?text=C',
    description: 'Description for Project C.',
  },
  {
    title: 'Project D',
    image: 'https://via.placeholder.com/200x200?text=D',
    description: 'Description for Project D.',
  },
  {
    title: 'Project E',
    image: 'https://via.placeholder.com/200x200?text=E',
    description: 'Description for Project E.',
  },
])

const activeProject = ref(null)

function openProject(index) {
  activeProject.value = index
}

function closeModal() {
  activeProject.value = null
}
</script>

<style scoped>
.hex-clip {
  clip-path: polygon(25% 6.7%, 75% 6.7%, 100% 50%, 75% 93.3%, 25% 93.3%, 0% 50%);
}
.hex-border {
  clip-path: polygon(25% 6.7%, 75% 6.7%, 100% 50%, 75% 93.3%, 25% 93.3%, 0% 50%);
}
</style>

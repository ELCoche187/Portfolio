<template>
  <section id="resume" class="relative w-full bg-[#2e2f33] text-white py-24 font-sarpanch overflow-hidden">
    <!-- Top-left logo -->
    <img :src="HexLogo" alt="Logo Cluster" class="absolute top-6 left-6 z-20 w-12 h-12 object-contain" />

    <!-- Diagonal lines (right side) -->
    <div class="absolute top-0 right-0 h-full w-24 flex flex-col justify-center gap-4 pr-8 z-0 opacity-70">
      <div class="border-r-2 border-cyan-300 transform rotate-12 h-32"></div>
      <div class="border-r-2 border-cyan-300 transform rotate-12 h-32"></div>
      <div class="border-r-2 border-cyan-300 transform rotate-12 h-32"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 max-w-screen-lg mx-auto px-6 text-center">
      <h2 class="text-4xl font-bold mb-3">Resume</h2>
      <p class="text-gray-300 mb-10">View my resume as either video or pdf.</p>

      <!-- Buttons -->
      <div class="flex flex-col md:flex-row justify-center items-center gap-6">
        <button @click="showVideo = true" class="resume-btn">
          Video CV
        </button>

        <a
          href="/resume.pdf"
          download
          class="resume-btn"
        >
          Regular CV
        </a>
      </div>
    </div>

    <!-- Video Modal -->
    <div v-if="showVideo" class="fixed inset-0 z-50 bg-black bg-opacity-80 flex items-center justify-center">
      <div class="w-full max-w-3xl bg-gray-900 p-4 rounded-lg shadow-xl relative">
        <button @click="showVideo = false" class="absolute top-2 right-2 text-white text-2xl font-bold">&times;</button>
        <iframe
          class="w-full h-[400px] rounded-md"
          :src="youtubeEmbedUrl"
          title="Video CV"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import HexLogo from '@/assets/images/hex-one.png';

const showVideo = ref(false)
const youtubeEmbedUrl = 'https://www.youtube.com/embed/dQw4w9WgXcQ' 
</script>

<style scoped>
.resume-btn {
  @apply bg-white text-black font-bold px-6 py-3 rounded-lg shadow-md transition duration-200;
}
.resume-btn:hover {
  @apply bg-gray-300;
}
</style>

<template>
    <section class="relative w-full min-h-screen bg-gray-900 text-white font-sarpanch">
      <!-- Background overlay -->
      <div class="absolute inset-0 bg-gray-400 opacity-20 z-0"></div>
  
      <div class="relative z-10 flex flex-col md:flex-row items-center justify-center gap-10 px-6 py-16">
        <!-- Hexagon image -->
        <div class="w-60 h-60 hexagon overflow-hidden border-4 border-indigo-500">
          <img
            src="../assets/images/your-image.jpg"
            alt="Profile"
            class="object-cover w-full h-full"
          />
        </div>
  
        <!-- Text content -->
        <div class="max-w-xl text-center md:text-left">
          <h1 class="text-5xl font-bold mb-4">Mika Edling</h1>
          <h2 class="text-xl font-semibold mb-4">A bit about me</h2>
          <p class="text-gray-200 leading-relaxed">
            I am a calm, grounded individual who enjoys spending time with friends and exploring new places.
            I have a passion for learning and love meeting new people wherever life takes me. I grew up in Germany with
            strong ties to Denmark, as I am half Danish. At 23 years old, I am currently pursuing my studies at EASV.
          </p>
  
          <div class="flex gap-4 mt-6 justify-center md:justify-start flex-wrap">
            <Button label="Resume" bg="bg-indigo-700" />
            <Button label="Projects" bg="bg-violet-500" />
            <Button label="Contact" bg="bg-slate-300 text-black" />
            <Button label="Personal" bg="bg-cyan-300 text-black" />
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  // Button is a local component
  import Button from './HexButton.vue'
  </script>
  
  <style scoped>
  .hexagon {
    clip-path: polygon(
      25% 5%, 75% 5%, 100% 50%,
      75% 95%, 25% 95%, 0% 50%
    );
  }
  </style>
<script setup>
  import heroBg from '@/assets/images/background.png'
  import heroBg from '@/assets/images/transparent-gray.png'
</script>

<template>
  <section class="relative w-full min-h-screen font-sarpanch text-white overflow-hidden">
    <!-- Background Layer 1 -->
    <div class="absolute inset-0 bg-cover bg-center z-0" style="background-image: url('/portfolio/src/assets/images/background.png')"></div>

    <!-- Background Layer 2 (transparent overlay) -->
    <div class="absolute inset-0 bg-cover bg-center z-10 opacity-70" style="background-image: url(${heroBg})"></div>


    <!-- Main Content -->
    <div class="relative z-30 max-w-screen-xl mx-auto flex flex-col lg:flex-row items-center justify-center gap-12 px-6 py-28">
      <!-- Profile hexagon -->
      <div class="w-[260px] h-[300px] relative">
        <div class="absolute inset-0 border-4 border-blue-500 hex-border z-10"></div>
        <img
          src="https://via.placeholder.com/260x300"
          alt="Profile"
          class="w-full h-full object-cover hex-clip relative z-0"
        />
      </div>

      <!-- Text & buttons -->
      <div class="text-left max-w-xl">
        <h1 class="text-5xl font-bold mb-3">Miko Edling</h1>
        <h2 class="text-2xl font-semibold mb-4">A bit about me</h2>
        <p class="text-white text-base leading-relaxed mb-6">
          I am a calm, grounded individual who enjoys spending time with friends and exploring new places. I have a
          passion for learning and love meeting new people wherever life takes me. I grew up in Germany with strong ties
          to Denmark, as I am half Danish. At 23 years old, I am currently pursuing my studies at EASV.
        </p>

        <!-- Nav Buttons -->
        <div class="flex flex-wrap gap-4 mt-6">
          <a href="#resume" class="btn-hex bg-indigo-900 text-white">Resume</a>
          <a href="#projects" class="btn-hex bg-purple-600 text-white" >Projects</a>
          <a href="#contact" class="btn-hex bg-blue-200 text-white" >Contact</a>
          <a href="#personal" class="btn-hex bg-cyan-300 text-white">Personal</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hex-clip {
  clip-path: polygon(25% 6.7%, 75% 6.7%, 100% 50%, 75% 93.3%, 25% 93.3%, 0% 50%);
}
.hex-border {
  clip-path: polygon(25% 6.7%, 75% 6.7%, 100% 50%, 75% 93.3%, 25% 93.3%, 0% 50%);
}
.btn-hex {
  @apply px-6 py-3 text-sm font-bold uppercase transition duration-200;
  clip-path: polygon(20% 0%, 80% 0%, 100% 50%, 80% 100%, 20% 100%, 0% 50%);
}
.btn-hex:hover {
  opacity: 0.85;
}
</style>

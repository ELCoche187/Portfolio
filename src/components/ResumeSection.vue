<template>
    <section class="relative w-full bg-gray-800 text-white py-20 px-6 font-sarpanch overflow-hidden">
      <!-- Top-left hexagon cluster -->
      <div class="absolute top-6 left-6 flex flex-col items-start space-y-1">
        <div class="w-4 h-4 bg-violet-600 rotate-45"></div>
        <div class="flex space-x-1">
          <div class="w-4 h-4 bg-white rotate-45"></div>
          <div class="w-4 h-4 bg-white rotate-45"></div>
        </div>
      </div>
  
      <!-- Right diagonal lines -->
      <div class="absolute top-0 right-0 h-full w-20 flex flex-col justify-end items-end pr-2 pt-10 space-y-2">
        <div class="border-r-2 border-cyan-400 h-full transform rotate-[30deg] origin-top-right"></div>
        <div class="border-r-2 border-cyan-400 h-full transform rotate-[30deg] origin-top-right"></div>
        <div class="border-r-2 border-cyan-400 h-full transform rotate-[30deg] origin-top-right"></div>
      </div>
  
      <!-- Center content -->
      <div class="relative z-10 max-w-3xl mx-auto text-center">
        <h2 class="text-4xl md:text-5xl font-bold mb-4">Resume</h2>
        <p class="text-gray-300 mb-8">View my resume as either video or pdf.</p>
  
        <div class="flex justify-center gap-6 flex-wrap">
          <a
            href="/videos/video-cv.mp4"
            target="_blank"
            class="bg-white text-black px-6 py-3 rounded-lg font-bold shadow-md hover:scale-105 transition"
          >
            Video CV
          </a>
          <a
            href="/files/resume.pdf"
            download
            class="bg-white text-black px-6 py-3 rounded-lg font-bold shadow-md hover:scale-105 transition"
          >
            Regular CV
          </a>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  // No script logic needed for this static section
  </script>
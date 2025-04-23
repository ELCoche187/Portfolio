<template>
    <section class="relative w-screen bg-gradient-to-br from-gray-900 to-gray-800 text-white py-20 px-6 font-sarpanch overflow-hidden">
      <!-- Hexagon cluster in corner -->
      <div class="absolute top-6 left-6 flex flex-col items-start space-y-1">
        <div class="w-4 h-4 bg-violet-600 rotate-45"></div>
        <div class="flex space-x-1">
          <div class="w-4 h-4 bg-white rotate-45"></div>
          <div class="w-4 h-4 bg-white rotate-45"></div>
        </div>
      </div>
  
      <!-- Heading -->
      <div class="text-center mb-12">
        <h2 class="text-4xl md:text-5xl font-bold">Projects</h2>
        <p class="text-gray-300 mt-2">Press the figures to gain more information</p>
      </div>
  
      <!-- Project hex grid -->
      <div class="flex justify-center flex-wrap gap-6">
        <ProjectHex
          v-for="(project, index) in projects"
          :key="index"
          :img="project.img"
          :label="project.label"
          :link="project.link"
          :border="project.border"
        />
      </div>
  
      <!-- More link -->
      <div class="text-right mt-10 pr-10">
        <a href="/projects" class="text-white text-xl inline-flex items-center hover:underline">
          More
          <span class="ml-2 text-3xl font-light">&rarr;</span>
        </a>
      </div>
    </section>
  </template>
  
  <script setup>
  import ProjectHex from './ProjectHex.vue'
  
  const projects = [
    {
      img: '/assets/images/project-1.jpg',
      label: 'Read more',
      link: '#',
      border: 'border-violet-500'
    },
    {
      img: '/assets/images/project-2.jpg',
      label: '',
      link: '#',
      border: 'border-sky-400'
    },
    {
      img: '/assets/images/project-3.jpg',
      label: '',
      link: '#',
      border: 'border-violet-400'
    },
    {
      img: '/assets/images/project-4.jpg',
      label: '',
      link: '#',
      border: 'border-cyan-300'
    }
  ]
  </script>
  
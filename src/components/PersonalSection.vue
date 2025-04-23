<template>
    <section class="relative w-full bg-gray-100 py-20 px-6 font-sarpanch text-white overflow-hidden" style="background-image: url('/assets/images/bg-hex-pattern.png'); background-size: cover;">
      <!-- Top-left hex cluster -->
      <div class="absolute top-6 left-6 flex flex-col items-start space-y-1 z-10">
        <div class="w-4 h-4 bg-violet-600 rotate-45"></div>
        <div class="flex space-x-1">
          <div class="w-4 h-4 bg-indigo-300 rotate-45"></div>
          <div class="w-4 h-4 bg-cyan-300 rotate-45"></div>
        </div>
      </div>
  
      <!-- Main content box -->
      <div class="bg-gray-700 bg-opacity-90 max-w-4xl mx-auto rounded-2xl p-8 md:p-12 space-y-6 relative z-10 shadow-xl">
        <h2 class="text-4xl font-bold text-white mb-4">Personal</h2>
  
        <div class="space-y-4">
          <Section
            title="About Me"
            content="Hi, I'm Mika Edling, a student and network agent for EASV with a passion for continuous learning and growth. My expertise lies in multimedia, and I thrive in team-oriented environments where I can apply my skills in communication, teamwork, and problem-solving. I'm proficient in Adobe programs and love working with people to bring creative projects to life."
          />
          <Section
            title="Interests & Hobbies"
            content="Cooking, Traveling\nPassionate about experiencing new cultures and flavors."
          />
          <Section
            title="Values & Philosophy"
            content="“Life has no limitations, except the ones you make.”\nAlways striving for a brighter future through knowledge and innovation."
          />
          <Section
            title="Volunteer Work & Social Impact"
            content="Greenpeace Collaboration – Contributed to a project focused on sustainability.\nDedicated to making a difference through creativity and teamwork."
          />
          <div>
            <h3 class="text-xl text-pink-300 font-semibold mb-2">Fun Extras</h3>
            <p class="mb-1">Favorite music genre: Depends on my mood, but rock always does the job.</p>
            <p class="mb-1">Favorite book: Erebos</p>
            <p class="font-semibold">Bucket List Goals:</p>
            <ul class="list-disc list-inside ml-4 space-y-1 text-white">
              <li>Climb the Himalayas</li>
              <li>Go skydiving from 5+ km</li>
              <li>Find a cure for lactose intolerance</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import Section from './PersonalSectionBlock.vue'
  </script>
  
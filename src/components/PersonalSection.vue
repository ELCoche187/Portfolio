<script setup>
  import HexLogo from '@/assets/images/hex-four.png'
</script>

<template>
  <section id="personal" class="relative bg-[#2e2f33] text-white py-24 font-sarpanch overflow-hidden">
    <div class="absolute inset-0  z-0 backgroundPerson"></div>
    <!-- Top-left logo -->
    <img :src="HexLogo" alt="Logo Cluster" class="absolute top-6 left-6 z-20 w-12 h-12 object-contain" />

    <div class="relative z-10 max-w-4xl mx-auto bg-[#20222b] bg-opacity-90 p-10 rounded-2xl shadow-lg">
      <h2 class="text-4xl font-bold mb-8 text-center">Personal</h2>

      <div class="space-y-8 text-gray-200">
        <!-- About -->
        <div>
          <h3 class="text-xl text-pink-300 font-semibold mb-2">About Me</h3>
          <p>
            Hi, I'm Mika Edling, a student and network agent for EASV with a passion for continuous learning and growth.
            I thrive in team-oriented environments where I can apply my communication and creative skills, particularly with Adobe software.
          </p>
        </div>

        <!-- Interests -->
        <div>
          <h3 class="text-xl text-pink-300 font-semibold mb-2">Interests & Hobbies</h3>
          <p>Cooking and traveling — passionate about experiencing new cultures and flavors.</p>
        </div>

        <!-- Philosophy -->
        <div>
          <h3 class="text-xl text-pink-300 font-semibold mb-2">Values & Philosophy</h3>
          <p>“Life has no limitations, except the ones you make.”</p>
        </div>

        <!-- Volunteer -->
        <div>
          <h3 class="text-xl text-pink-300 font-semibold mb-2">Volunteer Work & Social Impact</h3>
          <p>Worked with Greenpeace on sustainability-focused initiatives. I aim to make a difference through creativity and teamwork.</p>
        </div>

        <!-- Fun Extras -->
        <div>
          <h3 class="text-xl text-pink-300 font-semibold mb-2">Fun Extras</h3>
          <p class="mb-2">🎵 Favorite music: Rock (but depends on the mood)</p>
          <p class="mb-2">📚 Favorite book: Erebos</p>
          <p class="mb-1 font-semibold">📌 Bucket List:</p>
          <ul class="list-disc list-inside space-y-1 ml-4">
            <li>Climb the Himalayas</li>
            <li>Go skydiving from 5+ km</li>
            <li>Find a cure for lactose intolerance</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Uses Tailwind for styling — clean and responsive */
</style>

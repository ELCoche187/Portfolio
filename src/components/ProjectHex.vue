<template>
    <a
      :href="link"
      class="w-[220px] h-[220px] relative hex overflow-hidden transition-transform hover:scale-105 shadow-lg"
      :class="border"
    >
      <img :src="img" alt="Project" class="object-cover w-full h-full" />
      <div
        v-if="label"
        class="absolute bottom-3 right-3 bg-yellow-400 text-black px-2 py-1 text-xs font-bold rounded"
      >
        {{ label }}
      </div>
    </a>
  </template>
  
  <script setup>
  defineProps({
    img: String,
    label: String,
    link: String,
    border: String
  })
  </script>
  
  <style scoped>
  .hex {
    clip-path: polygon(
      25% 5%, 75% 5%, 100% 50%,
      75% 95%, 25% 95%, 0% 50%
    );
  }
  </style>
  
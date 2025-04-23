<template>
    <button
      :class="[
        'hex-button px-6 py-2 font-bold text-sm uppercase transition-transform duration-300 hover:scale-105',
        bg,
      ]"
    >
      {{ label }}
    </button>
  </template>
  
  <script setup>
  defineProps({
    label: String,
    bg: {
      type: String,
      default: 'bg-indigo-500'
    }
  })
  </script>
  
  <style scoped>
  .hex-button {
    clip-path: polygon(
      25% 0%, 75% 0%, 100% 50%,
      75% 100%, 25% 100%, 0% 50%
    );
  }
  </style>
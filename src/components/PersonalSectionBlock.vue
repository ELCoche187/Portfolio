<template>
    <div>
      <h3 class="text-xl text-pink-300 font-semibold mb-2">{{ title }}</h3>
      <p class="whitespace-pre-line text-white">{{ content }}</p>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    content: String,
  })
  </script>
  
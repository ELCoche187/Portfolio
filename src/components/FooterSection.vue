<template>
    <footer class="relative bg-gray-900 text-white font-sarpanch py-6 px-4">
      <!-- Top-left hex cluster -->
    
  
      <div class="max-w-5xl mx-auto flex flex-col sm:flex-row justify-between items-center text-sm">
        <p class="text-gray-300">&copy; {{ year }} Mika Edling. All rights reserved.</p>
  
        <div class="flex items-center gap-4 mt-2 sm:mt-0">
          <a
            href="mailto:mikaedling@gmail.com"
            class="hover:underline text-gray-300"
          >
            Email
          </a>
          <a
            href="https://www.linkedin.com/in/miko-edling-825400280"
            target="_blank"
            class="hover:underline text-gray-300"
          >
            LinkedIn
          </a>
        </div>
      </div>
    </footer>
  </template>
  
  <script setup>
  const year = new Date().getFullYear()
  </script>
  
<script setup>
import HexLogo from '@/assets/images/hex-three.png'
</script>

<template>
  <section id="contact" class="relative w-7xl bg-[#2e2f33] text-white py-24 font-sarpanch">
    <!-- Top-left logo -->
    <img :src="HexLogo" alt="Logo Cluster" class="absolute top-6 left-6 z-20 w-12 h-12 object-contain" />

    <div class="relative z-10 max-w-screen-md mx-auto px-6 text-center">
      <h2 class="text-4xl font-bold mb-3">Contact</h2>

      <ul class="space-y-6 text-lg">
        <li class="flex items-center gap-4">
          <span class="text-xl">👤</span>
          <span>Miko Edling</span>
        </li>
        <li class="flex items-center gap-4">
          <span class="text-xl">🏠</span>
          <span>Finsensgade 18, 1th</span>
        </li>
        <li class="flex items-center gap-4">
          <span class="text-xl">🏢</span>
          <span>Esbjerg 6700</span>
        </li>
        <li class="flex items-center gap-4">
          <span class="text-xl">📞</span>
          <span>+45 93 91 87 69</span>
        </li>
        <li class="flex items-center gap-4">
          <span class="text-xl">✉️</span>
          <span>mikaedling@gmail.com</span>
        </li>
        <li class="flex items-center gap-4">
          <span class="text-xl">🔗</span>
          <a href="https://linkedin.com/in/mika-edling" target="_blank" class="text-green-400 hover:underline">
            linkedin.com/in/mika-edling
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
ul li span {
  font-size: 1rem;
}
</style>

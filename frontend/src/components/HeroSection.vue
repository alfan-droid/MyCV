<script setup>
import fotoProfil from '@/assets/profil.jpg';
</script>
<template>
  <section id="profil" class="bg-slate-900">
    <div class="container mx-auto px-6 py-20 flex flex-col md:flex-row items-center">
      <div class="md:w-1/2 mb-10 md:mb-0">
        <h1 class="text-5xl font-bold text-white mb-4 animate-slide-in-left" style="animation-delay: 200ms;">
          Halo, Saya <span class="text-sky-500">Alfan</span>
        </h1>
        <p class="text-xl text-slate-400 mb-8 animate-slide-in-left" style="animation-delay: 400ms;">
          Mahasiswa Informatika yang bersemangat dalam pengembangan web dan desain antarmuka.
        </p>
        <a href="#kontak" class="bg-sky-500 text-white font-bold py-3 px-6 rounded-lg hover:bg-sky-600 transition-colors duration-300 inline-block animate-slide-in-left" style="animation-delay: 600ms;">
          Hubungi Saya
        </a>
      </div>
      <div class="md:w-1/2 flex justify-center animate-slide-in-right">
        <img :src="fotoProfil" alt="Foto Profil" class="w-80 h-80 rounded-full object-cover shadow-lg shadow-sky-900/20">
      </div>
    </div>
  </section>
</template>
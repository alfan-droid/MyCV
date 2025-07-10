<script setup>
import SectionTitle from './SectionTitle.vue';
const educationHistory = [
  { id: 1, period: '2023 - Sekarang', institution: 'Universitas Amikom Yogyakarta', major: 'S1 - Informatika' },
  { id: 2, period: '2020 - 2023', institution: 'SMA IT AL HUDA WONOGIRI', major: 'MIPA' }
];
</script>
<template>
  <section id="pendidikan" class="py-20 bg-slate-800">
    <div class="container mx-auto px-6">
      <SectionTitle title="Riwayat Pendidikan" />
      <div class="relative">
        <div class="absolute h-full border-r-2 border-slate-600" style="left: 50%;"></div>
        <div v-for="(edu, index) in educationHistory" :key="edu.id" class="mb-8 flex justify-between items-center w-full">
          <div v-if="index % 2 === 0" class="w-full flex">
            <div class="w-1/2 pr-8 text-right">
              <p class="font-semibold text-sky-400">{{ edu.period }}</p>
              <h3 class="text-2xl font-bold text-white">{{ edu.institution }}</h3>
              <p class="text-slate-400">{{ edu.major }}</p>
            </div>
            <div class="w-1/2 flex justify-start">
              <div class="w-4 h-4 bg-sky-500 rounded-full z-10 ring-8 ring-slate-800"></div>
            </div>
          </div>
          <div v-else class="w-full flex">
            <div class="w-1/2 flex justify-end">
              <div class="w-4 h-4 bg-sky-500 rounded-full z-10 ring-8 ring-slate-800"></div>
            </div>
            <div class="w-1/2 pl-8 text-left">
              <p class="font-semibold text-sky-400">{{ edu.period }}</p>
              <h3 class="text-2xl font-bold text-white">{{ edu.institution }}</h3>
              <p class="text-slate-400">{{ edu.major }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
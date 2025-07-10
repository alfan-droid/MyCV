<script setup>
import SectionTitle from './SectionTitle.vue';
import kedaikopiImage from '@/assets/kedaikopi.jpg';
import FiveAlignImage from '@/assets/FiveAlign.jpg';
const projects = [
  // Proyek Baru Ditambahkan
  { 
    title: 'Website Kedai Kopi Kayu', 
    image: kedaikopiImage,
    description: 'Website company profile untuk kedai kopi dengan desain modern dan informasi produk.', 
    tech: ['HTML5', 'CSS3', 'JavaScript'], 
    link: 'https://kedaikopikayu.my.id/' 
  },
  {
    title: 'Five Align',
    image: FiveAlignImage,
    description: 'A structured daily ritual designed to synchronize inner peace and productivity through five mindful pauses in a day.',
    tech: ['Iman','Taqwa'],
    link: 'https://www.google.com/search?q=sholat&oq=sholat&gs_lcrp=EgZjaHJvbWUyDAgAEEUYORixAxiABDIPCAEQABhDGLEDGIAEGIoFMgoIAhAAGLEDGIAEMg0IAxAAGLEDGIAEGIoFMgoIBBAAGLEDGIAEMgoIBRAAGLEDGIAEMgYIBhBFGD0yBggHEEUYPNIBCDM3NzFqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8'
  }
];
</script>
<template>
  <section id="proyek" class="py-20 bg-slate-800">
    <div class="container mx-auto px-6">
      <SectionTitle title="Proyek Unggulan" />
      <div class="grid md:grid-cols-2 gap-12">
        <div v-for="project in projects" :key="project.title" class="bg-slate-900 rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition-transform duration-300">
          <img :src="project.image" alt="Gambar Proyek" class="w-full h-56 object-cover">
          <div class="p-6">
            <h3 class="text-2xl font-bold text-white mb-2">{{ project.title }}</h3>
            <p class="text-slate-400 mb-4">{{ project.description }}</p>
            <div class="mb-4">
              <span v-for="t in project.tech" :key="t" class="inline-block bg-sky-900/50 text-sky-300 text-sm font-semibold mr-2 mb-2 px-2.5 py-0.5 rounded-full">{{ t }}</span>
            </div>
            <a :href="project.link" target="_blank" rel="noopener noreferrer" class="text-sky-400 font-semibold hover:underline">Lihat Detail &rarr;</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
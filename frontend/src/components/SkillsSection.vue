<script setup>
// import SectionTitle from './SectionTitle.vue';
// const skills = [
//   { name: 'Vue.js', level: 'Bisa' }, { name: 'JavaScript', level: 'Bisa Mati' },
//   { name: 'Tailwind CSS', level: 'Ya Allah' }, { name: 'Node.js', level: 'Udah Bang' },
//   { name: 'Express.js', level: 'Pengen Pulang' }, { name: 'PostgreSQL', level: 'Ckptw' },
//   { name: 'Git & GitHub', level: 'Apa ini' }, { name: 'HTML5 & CSS3', level: 'Mahir' },
// ];

import { ref, onMounted } from 'vue';
import axios from 'axios';
import SectionTitle from './SectionTitle.vue';
const skills = ref([]);
onMounted(async () => {
try { const response = await axios.get('http://localhost:3000/api/skills'); skills.value = response.data;
} catch (error) { console.error(error); }
});

</script>
<template>
  <section id="skill" class="py-20 bg-slate-900">
    <div class="container mx-auto px-6">
      <SectionTitle title="Keahlian & Teknologi" />
      <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
        <div v-for="skill in skills" :key="skill.name" class="bg-slate-800 p-6 rounded-lg shadow-lg text-center transform hover:-translate-y-2 transition-all duration-300 hover:shadow-sky-500/20 hover:ring-2 hover:ring-sky-500">
          <h3 class="text-xl font-bold text-white">{{ skill.name }}</h3>
          <p class="text-slate-400 mt-2">{{ skill.level }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
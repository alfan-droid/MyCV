<script setup>
import Navbar from '@/components/NavbarSection.vue';
import Hero from '@/components/HeroSection.vue';
import SkillsSection from '@/components/SkillsSection.vue';
import ProjectsSection from '@/components/ProjectsSection.vue';
import ContactSection from '@/components/ContactSection.vue';
import EducationSection from '@/components/EducationSection.vue';
</script>
<template>
<div>
<Navbar />
<main>
<Hero />
<div v-animate-on-scroll><EducationSection /></div>
<div v-animate-on-scroll><SkillsSection /></div>
<div v-animate-on-scroll><ProjectsSection /></div>
<div v-animate-on-scroll><ContactSection /></div>
</main>
</div>
</template>
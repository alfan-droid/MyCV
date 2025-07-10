<script setup>
import SectionTitle from './SectionTitle.vue';
</script>
<template>
  <footer id="kontak" class="py-20 bg-slate-900 text-white">
    <div class="container mx-auto px-6 text-center">
      <SectionTitle title="Hubungi Saya" />
      <p class="text-xl text-slate-300 mb-8">Jangan ragu untuk terhubung atau bertanya.</p>
      
      <a href="mailto:alfanshob2980@gmail.com" class="bg-sky-500 text-white font-bold py-3 px-6 rounded-lg hover:bg-sky-600 transition-colors duration-300 inline-block mb-12">
        Kirim Email
      </a>
      
      <div class="flex justify-center space-x-6 mb-8">
        <a href="https://github.com/alfan-droid" target="_blank" rel="noopener noreferrer" class="text-slate-400 hover:text-sky-400 transition-colors duration-300" title="GitHub">
          <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.168 6.839 9.492.5.092.682-.217.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.378.203 2.398.1 2.651.64.7 1.03 1.595 1.03 2.688 0 3.848-2.338 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12c0-5.523-4.477-10-10-10z" clip-rule="evenodd" /></svg>
        </a>
        <a href="https://wa.me/6285920014454" target="_blank" rel="noopener noreferrer" class="text-slate-400 hover:text-sky-400 transition-colors duration-300" title="WhatsApp">
          <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M12.04 2c-5.46 0-9.91 4.45-9.91 9.91 0 1.75.46 3.45 1.32 4.95L2 22l5.25-1.38c1.45.79 3.08 1.21 4.79 1.21h.01c5.46 0 9.91-4.45 9.91-9.91s-4.45-9.91-9.91-9.91zM17.5 14.3c-.28-.14-1.67-.82-1.93-.91s-.45-.14-.64.14-.73.91-.9 1.1s-.33.21-.61.07c-.28-.14-1.18-.44-2.25-1.39s-1.76-2.04-1.96-2.4c-.2-.35-.01-.54.12-.68.12-.12.28-.33.42-.49s.18-.28.28-.47.05-.35-.02-.49c-.07-.14-.64-1.54-.88-2.1s-.48-.48-.64-.49-.35-.01-.53-.01h-.45c-.18 0-.47.07-.71.35s-.96.94-.96 2.28.98 2.65 1.13 2.83c.14.18 1.96 3.01 4.76 4.22.62.27 1.1.43 1.48.55.57.19 1.07.16 1.46.1.44-.07 1.39-.57 1.58-1.12s.19-.99.13-1.12-.18-.18-.46-.32z"/></svg>
        </a>
        <a href="https://www.instagram.com/alfan_shob/?__pwa=1#" target="_blank" rel="noopener noreferrer" class="text-slate-400 hover:text-sky-400 transition-colors duration-300" title="Instagram">
          <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M12 2C8.134 2 6 4.134 6 8v8c0 3.866 2.134 6 6 6s6-2.134 6-6V8c0-3.866-2.134-6-6-6zm4 11a4 4 0 11-8 0 4 4 0 018 0zm-2 0a2 2 0 11-4 0 2 2 0 014 0z" clip-rule="evenodd" /></svg>
        </a>
      </div>
      
      <p class="text-slate-500">&copy; {{ new Date().getFullYear() }} Alfan. Dibuat dengan Vue.js & Tailwind CSS.</p>
    </div>
  </footer>
</template>
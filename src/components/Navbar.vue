<script setup>
import { ref, onMounted, onUnmounted } from 'vue';

const isScrolled = ref(false);

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50;
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});

const navLinks = [
  { name: 'Home', href: '#home' },
  { name: 'Services', href: '#services' },
  { name: 'Projects', href: '#projects' },
  { name: 'About', href: '#about' },
  { name: 'Contact', href: '#contact' },
];
</script>

<template>
  <nav 
    :class="[
      'fixed w-full z-50 transition-all duration-300',
      isScrolled ? 'bg-black/95 backdrop-blur-md py-4 shadow-[0_4px_30px_rgba(29,94,65,0.2)] border-b border-brand-green/30' : 'bg-transparent py-6'
    ]"
  >
    <div class="max-w-7xl mx-auto px-6 flex justify-between items-center">
      <!-- Logo placeholder if image is missing, utilizing the font -->
      <a href="#home" class="flex items-center gap-2 group">
        <div class="text-brand-green font-heading text-4xl leading-none group-hover:text-green-500 transition-colors">ME</div>
        <div class="flex flex-col">
          <span class="font-body text-white text-sm uppercase tracking-widest leading-none">Metalúrgica</span>
          <span class="font-heading text-brand-gray text-xl leading-none">Eblagon</span>
        </div>
      </a>

      <!-- Desktop Links -->
      <div class="hidden md:flex items-center gap-8">
        <a 
          v-for="link in navLinks" 
          :key="link.name"
          :href="link.href"
          class="font-body text-brand-gray hover:text-brand-green uppercase text-sm tracking-wider transition-colors"
        >
          {{ link.name }}
        </a>
      </div>

      <!-- Mobile menu button (simple) -->
      <button class="md:hidden text-white hover:text-brand-green">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
        </svg>
      </button>
    </div>
  </nav>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  icon: String,
});
</script>

<template>
  <div class="group relative bg-[#0a0a0a] border border-[#222] p-8 transition-all duration-500 hover:-translate-y-2 hover:border-brand-green">
    <!-- Accent line -->
    <div class="absolute top-0 left-0 w-full h-1 bg-[#222] transition-colors duration-500 group-hover:bg-brand-green"></div>
    
    <div class="text-4xl mb-6 text-brand-gray group-hover:text-white transition-colors duration-500">
      {{ icon }}
    </div>
    
    <h3 class="text-2xl font-heading text-white mb-4 group-hover:text-brand-green transition-colors duration-300">
      {{ title }}
    </h3>
    
    <p class="font-body text-sm text-brand-gray leading-relaxed">
      {{ description }}
    </p>
    
    <!-- Decorative corner bracket -->
    <div class="absolute bottom-0 right-0 w-8 h-8 border-b-2 border-r-2 border-transparent transition-colors duration-500 group-hover:border-brand-green"></div>
  </div>
</template>

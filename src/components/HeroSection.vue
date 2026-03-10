<script setup>
// Hero Section Component
</script>

<template>
  <section id="home" class="relative min-h-screen flex items-center justify-center overflow-hidden bg-black">
    <!-- Industrial Texture Background (simulated with CSS patterns) -->
    <div class="absolute inset-0 opacity-20 bg-[radial-gradient(#1d5e41_1px,transparent_1px)] [background-size:20px_20px]"></div>
    <div class="absolute inset-0 bg-gradient-to-b from-black/60 via-black/80 to-black"></div>
    
    <div class="relative z-10 max-w-5xl mx-auto px-6 text-center mt-20">
      <div class="animate-fade-in-up">
        <span class="font-body text-brand-green text-lg md:text-xl uppercase tracking-[0.3em] mb-4 block">
          Industrial Excellence
        </span>
        <h1 class="text-5xl md:text-7xl lg:text-8xl font-heading text-white mb-8 leading-tight tracking-wider">
          Precision Metal <br/>
          <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-green to-green-400">
            Fabrication
          </span> 
          <br/> in Córdoba
        </h1>
        <p class="font-body text-brand-gray max-w-2xl mx-auto mb-12 text-lg leading-relaxed">
          High-quality metal structures, laser cutting, and custom industrial parts manufactured with absolute precision and speed.
        </p>
        <div class="flex flex-col sm:flex-row justify-center gap-6">
          <a href="#contact" class="btn-primary">
            Request a Quote
          </a>
          <a href="#services" class="btn-outline">
            Our Services
          </a>
        </div>
      </div>
    </div>
    
    <!-- Scroll down indicator -->
    <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
      <a href="#services" class="text-brand-gray hover:text-brand-green transition-colors">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3" />
        </svg>
      </a>
    </div>
  </section>
</template>

<style scoped>
.animate-fade-in-up {
  animation: fadeInUp 1s ease-out forwards;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

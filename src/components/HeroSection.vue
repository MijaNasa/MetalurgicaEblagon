<script setup>
// Hero Section - Metalúrgica Eblagon
</script>

<template>
  <section id="home" class="relative min-h-screen flex items-center overflow-hidden bg-black">
    <!-- Background Image -->
    <div 
      class="absolute inset-0 bg-cover bg-center bg-no-repeat"
      style="background-image: url('/hero-bg.png');"
    ></div>
    <!-- Dark overlay + gradient -->
    <div class="absolute inset-0 bg-gradient-to-r from-black/90 via-black/70 to-black/40"></div>
    <div class="absolute inset-0 bg-gradient-to-t from-black via-transparent to-black/60"></div>

    <!-- Blue-ish border glow at bottom -->
    <div class="absolute bottom-0 left-0 right-0 h-px bg-gradient-to-r from-transparent via-brand-green to-transparent opacity-60"></div>

    <!-- Content -->
    <div class="relative z-10 max-w-7xl mx-auto px-6 pt-28 pb-16 grid grid-cols-1 lg:grid-cols-2 gap-12 items-center w-full">
      <!-- Left: Text -->
      <div class="animate-fade-in-up">
        <p class="font-body text-brand-green text-sm uppercase tracking-[0.35em] mb-6">
          Córdoba, Argentina
        </p>

        <h1 class="font-heading text-white text-5xl md:text-7xl leading-[0.9] uppercase mb-8">
          METALURGICA<br/>
          <span class="text-brand-green">EBLAGON</span>
        </h1>

        <p class="font-body text-white/60 max-w-md text-base leading-relaxed mb-10">
          Mecanizado de piezas y fabricación de cuchillas para cortadoras de fiambre.
        </p>

        <div class="flex flex-wrap gap-4">
          <a
            href="#contact"
            class="flex items-center gap-3 bg-brand-green hover:bg-[#164d33] text-white font-heading text-sm uppercase tracking-widest px-8 py-4 rounded-full transition-all duration-300 shadow-[0_0_30px_rgba(29,94,65,0.6)] hover:shadow-[0_0_50px_rgba(29,94,65,0.8)] hover:scale-105"
          >
            PEDIR PRESUPUESTO
            <svg class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
          </a>
          <a
            href="#services"
            class="flex items-center gap-2 border border-white/30 hover:border-brand-green text-white hover:text-brand-green font-heading text-sm uppercase tracking-widest px-8 py-4 rounded-full transition-all duration-300"
          >
            Ver Servicios
          </a>
        </div>

        <!-- Stats bar -->
        <div class="mt-14 flex gap-10 border-t border-white/10 pt-8">
          <div>
            <div class="font-heading text-brand-green text-3xl">20+</div>
            <div class="font-body text-white/40 text-xs uppercase tracking-wider mt-1">Años de Trayectoria</div>
          </div>
          <div>
            <div class="font-heading text-brand-green text-3xl">5K+</div>
            <div class="font-body text-white/40 text-xs uppercase tracking-wider mt-1">Proyectos Entregados</div>
          </div>
          <div>
            <div class="font-heading text-brand-green text-3xl">100%</div>
            <div class="font-body text-white/40 text-xs uppercase tracking-wider mt-1">Satisfacción</div>
          </div>
        </div>
      </div>

      <!-- Right: Logo Card -->
      <div class="hidden lg:flex justify-center items-center animate-fade-in-right">
        <div class="relative bg-brand-green/10 border border-brand-green/30 rounded-2xl p-10 backdrop-blur-sm shadow-[0_0_60px_rgba(29,94,65,0.3)]">
          <div class="absolute inset-0 rounded-2xl bg-gradient-to-br from-brand-green/20 to-transparent"></div>
          <div class="relative flex flex-col items-center gap-4 p-4">
            <img
              src="/logo.png"
              alt="Metalúrgica Eblagon"
              class="w-80 h-auto object-contain rounded-xl"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Scroll down arrow -->
    <div class="absolute bottom-8 left-1/2 -translate-x-1/2 animate-bounce z-10">
      <a href="#services" class="text-white/30 hover:text-brand-green transition-colors">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M19 9l-7 7-7-7"/>
        </svg>
      </a>
    </div>
  </section>
</template>

<style scoped>
.animate-fade-in-up {
  animation: fadeInUp 0.9s ease-out forwards;
}
.animate-fade-in-right {
  animation: fadeInRight 1.1s ease-out 0.2s both;
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(40px); }
  to { opacity: 1; transform: translateY(0); }
}
@keyframes fadeInRight {
  from { opacity: 0; transform: translateX(40px); }
  to { opacity: 1; transform: translateX(0); }
}
</style>

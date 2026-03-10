<template>
  <section id="why-us" class="relative bg-black overflow-hidden">
    <!-- Background with industrial image overlay -->
    <div class="absolute inset-0 bg-cover bg-center bg-no-repeat opacity-20" style="background-image: url('/hero-bg.png');"></div>
    <div class="absolute inset-0 bg-gradient-to-r from-black via-black/80 to-black/60"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 py-24">
      <!-- Header -->
      <div class="mb-16">
        <p class="font-body text-brand-green text-xs uppercase tracking-[0.3em] mb-4">Por qué Elegirnos</p>
        <div class="flex items-baseline gap-4">
          <span class="font-heading text-brand-green/20 text-[120px] leading-none select-none">04</span>
          <h2 class="font-heading text-white text-4xl md:text-6xl uppercase leading-tight">
            RAZONES
          </h2>
        </div>
        <p class="font-body text-white/40 mt-2 text-sm max-w-sm">Por qué los clientes más exigentes confían en Metalúrgica Eblagon.</p>
      </div>

      <!-- Cards Grid -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-5">

        <!-- Card 1 -->
        <div class="group bg-white/5 border border-white/10 hover:border-brand-green/40 rounded-2xl p-8 transition-all duration-300 hover:-translate-y-1 hover:shadow-[0_8px_30px_rgba(29,94,65,0.2)]">
          <div class="w-12 h-12 rounded-xl bg-brand-green/10 group-hover:bg-brand-green/20 flex items-center justify-center mb-5 transition-all">
            <svg class="w-6 h-6 text-brand-green" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 12L3.269 3.126A59.768 59.768 0 0121.485 12 59.77 59.77 0 013.27 20.876L5.999 12zm0 0h7.5"/>
            </svg>
          </div>
          <h3 class="font-heading text-white text-xl uppercase mb-3 group-hover:text-brand-green transition-colors">Precisión Industrial</h3>
          <p class="font-body text-white/50 text-sm leading-relaxed">Equipamiento de última generación que garantiza exactitud micrométrica en cada proyecto.</p>
        </div>

        <!-- Card 2 -->
        <div class="group bg-white/5 border border-white/10 hover:border-brand-green/40 rounded-2xl p-8 transition-all duration-300 hover:-translate-y-1 hover:shadow-[0_8px_30px_rgba(29,94,65,0.2)]">
          <div class="w-12 h-12 rounded-xl bg-brand-green/10 group-hover:bg-brand-green/20 flex items-center justify-center mb-5 transition-all">
            <svg class="w-6 h-6 text-brand-green" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
              <path stroke-linecap="round" stroke-linejoin="round" d="M9.594 3.94c.09-.542.56-.94 1.11-.94h2.593c.55 0 1.02.398 1.11.94l.213 1.281c.063.374.313.686.645.87.074.04.147.083.22.127.324.196.72.257 1.075.124l1.217-.456a1.125 1.125 0 011.37.49l1.296 2.247a1.125 1.125 0 01-.26 1.431l-1.003.827c-.293.24-.438.613-.431.992a6.759 6.759 0 010 .255c-.007.378.138.75.43.99l1.005.828c.424.35.534.954.26 1.43l-1.298 2.247a1.125 1.125 0 01-1.369.491l-1.217-.456c-.355-.133-.75-.072-1.076.124a6.57 6.57 0 01-.22.128c-.331.183-.581.495-.644.869l-.213 1.28c-.09.543-.56.941-1.11.941h-2.594c-.55 0-1.02-.398-1.11-.94l-.213-1.281c-.062-.374-.312-.686-.644-.87a6.52 6.52 0 01-.22-.127c-.325-.196-.72-.257-1.076-.124l-1.217.456a1.125 1.125 0 01-1.369-.49l-1.297-2.247a1.125 1.125 0 01.26-1.431l1.004-.827c.292-.24.437-.613.43-.992a6.932 6.932 0 010-.255c.007-.378-.138-.75-.43-.99l-1.004-.828a1.125 1.125 0 01-.26-1.43l1.297-2.247a1.125 1.125 0 011.37-.491l1.216.456c.356.133.751.072 1.076-.124.072-.044.146-.087.22-.128.332-.183.582-.495.644-.869l.214-1.281z"/>
              <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/>
            </svg>
          </div>
          <h3 class="font-heading text-white text-xl uppercase mb-3 group-hover:text-brand-green transition-colors">Fabricación a Medida</h3>
          <p class="font-body text-white/50 text-sm leading-relaxed">Soluciones diseñadas específicamente para sus requerimientos únicos y planos técnicos.</p>
        </div>

        <!-- Card 3 -->
        <div class="group bg-white/5 border border-white/10 hover:border-brand-green/40 rounded-2xl p-8 transition-all duration-300 hover:-translate-y-1 hover:shadow-[0_8px_30px_rgba(29,94,65,0.2)]">
          <div class="w-12 h-12 rounded-xl bg-brand-green/10 group-hover:bg-brand-green/20 flex items-center justify-center mb-5 transition-all">
            <svg class="w-6 h-6 text-brand-green" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
              <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z"/>
            </svg>
          </div>
          <h3 class="font-heading text-white text-xl uppercase mb-3 group-hover:text-brand-green transition-colors">Entrega Rápida</h3>
          <p class="font-body text-white/50 text-sm leading-relaxed">Optimización de planta productiva que garantiza el cumplimiento estricto de plazos de entrega.</p>
        </div>

        <!-- Card 4 -->
        <div class="group bg-white/5 border border-white/10 hover:border-brand-green/40 rounded-2xl p-8 transition-all duration-300 hover:-translate-y-1 hover:shadow-[0_8px_30px_rgba(29,94,65,0.2)]">
          <div class="w-12 h-12 rounded-xl bg-brand-green/10 group-hover:bg-brand-green/20 flex items-center justify-center mb-5 transition-all">
            <svg class="w-6 h-6 text-brand-green" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15 19.128a9.38 9.38 0 002.625.372 9.337 9.337 0 004.121-.952 4.125 4.125 0 00-7.533-2.493M15 19.128v-.003c0-1.113-.285-2.16-.786-3.07M15 19.128v.106A12.318 12.318 0 018.624 21c-2.331 0-4.512-.645-6.374-1.766l-.001-.109a6.375 6.375 0 0111.964-3.07M12 6.375a3.375 3.375 0 11-6.75 0 3.375 3.375 0 016.75 0zm8.25 2.25a2.625 2.625 0 11-5.25 0 2.625 2.625 0 015.25 0z"/>
            </svg>
          </div>
          <h3 class="font-heading text-white text-xl uppercase mb-3 group-hover:text-brand-green transition-colors">Equipo Experimentado</h3>
          <p class="font-body text-white/50 text-sm leading-relaxed">Soldadores e ingenieros certificados con más de 20 años de experiencia en el sector.</p>
        </div>

      </div>
    </div>
  </section>
</template>

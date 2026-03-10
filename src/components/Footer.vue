<template>
  <footer class="bg-brand-green pt-16 pb-8">
    <div class="max-w-7xl mx-auto px-6">
      <!-- Top grid -->
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
        <!-- Brand -->
        <div class="md:col-span-1">
          <a href="#home" class="flex items-center gap-3 group mb-6">
            <div class="w-10 h-10 flex items-center justify-center border-2 border-white/40 rounded-full group-hover:border-white transition-all">
              <span class="font-heading text-white text-sm font-bold">ME</span>
            </div>
            <div class="flex flex-col leading-tight">
              <span class="font-heading text-white text-sm tracking-widest uppercase">Metalúrgica</span>
              <span class="font-body text-white/70 text-xs tracking-wider">Eblagon</span>
            </div>
          </a>
          <p class="font-body text-white/60 text-xs leading-relaxed max-w-xs">
            Fabricación metálica industrial y soluciones de ingeniería estructural para quienes exigen excelencia.
          </p>

          <!-- Social icons -->
          <div class="flex gap-3 mt-6">
            <a href="#" class="w-9 h-9 rounded-full bg-white/10 hover:bg-white hover:text-brand-green flex items-center justify-center text-white text-xs font-heading transition-all duration-300">
              <span>in</span>
            </a>
            <a href="#" class="w-9 h-9 rounded-full bg-white/10 hover:bg-white hover:text-brand-green flex items-center justify-center text-white text-xs font-heading transition-all duration-300">
              <span>ig</span>
            </a>
            <a href="#" class="w-9 h-9 rounded-full bg-white/10 hover:bg-white hover:text-brand-green flex items-center justify-center text-white text-xs font-heading transition-all duration-300">
              <span>fb</span>
            </a>
          </div>
        </div>

        <!-- Quick Links -->
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-sm uppercase tracking-widest mb-5">Navegación</h4>
          <ul class="space-y-3 font-body text-sm text-white/60">
            <li><a href="#home" class="hover:text-white transition-colors">Inicio</a></li>
            <li><a href="#services" class="hover:text-white transition-colors">Servicios</a></li>
            <li><a href="#projects" class="hover:text-white transition-colors">Proyectos</a></li>
            <li><a href="#about" class="hover:text-white transition-colors">Sobre Nosotros</a></li>
            <li><a href="#contact" class="hover:text-white transition-colors">Contacto</a></li>
          </ul>
        </div>

        <!-- Services -->
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-sm uppercase tracking-widest mb-5">Servicios</h4>
          <ul class="space-y-3 font-body text-sm text-white/60">
            <li><a href="#services" class="hover:text-white transition-colors">Corte Láser</a></li>
            <li><a href="#services" class="hover:text-white transition-colors">Plegado de Chapa</a></li>
            <li><a href="#services" class="hover:text-white transition-colors">Estructuras Metálicas</a></li>
            <li><a href="#services" class="hover:text-white transition-colors">Prototipos a Medida</a></li>
            <li><a href="#services" class="hover:text-white transition-colors">Acabado Superficial</a></li>
          </ul>
        </div>

        <!-- Newsletter / CTA -->
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-sm uppercase tracking-widest mb-5">Mantenete Informado</h4>
          <p class="font-body text-white/60 text-xs leading-relaxed mb-4">Suscribite para recibir novedades sobre nuestros servicios y proyectos.</p>
          <div class="flex gap-2">
            <input 
              type="email" 
              placeholder="tu@email.com" 
              class="flex-1 bg-white/10 border border-white/20 text-white placeholder-white/40 font-body text-xs px-4 py-3 rounded-full focus:outline-none focus:border-white/50 transition-all"
            />
            <button class="bg-white text-brand-green font-heading text-xs uppercase px-4 py-3 rounded-full hover:bg-white/90 transition-all">
              OK
            </button>
          </div>
        </div>
      </div>

      <!-- Bottom bar -->
      <div class="border-t border-white/20 pt-8 flex flex-col md:flex-row justify-between items-center gap-4">
        <p class="font-body text-white/40 text-xs uppercase tracking-widest">
          © {{ new Date().getFullYear() }} Metalúrgica Eblagon. Todos los derechos reservados.
        </p>
        <div class="flex gap-6 font-body text-white/40 text-xs">
          <a href="#" class="hover:text-white transition-colors">Política de Privacidad</a>
          <a href="#" class="hover:text-white transition-colors">Términos de Servicio</a>
        </div>
      </div>
    </div>
  </footer>
</template>

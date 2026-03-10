<template>
  <footer class="bg-black border-t-4 border-brand-green pt-16 pb-8">
    <div class="max-w-7xl mx-auto px-6">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
        
        <div class="md:col-span-1">
          <a href="#home" class="flex items-center gap-2 group mb-6">
            <div class="text-brand-green font-heading text-4xl leading-none group-hover:text-green-500 transition-colors">ME</div>
            <div class="flex flex-col">
              <span class="font-body text-white text-sm uppercase tracking-widest leading-none">Metalúrgica</span>
              <span class="font-heading text-brand-gray text-xl leading-none">Eblagon</span>
            </div>
          </a>
          <p class="font-body text-xs text-[#555] leading-relaxed mb-6 max-w-xs">
            Industrial metal fabrication and structural engineering solutions for professionals who demand excellence.
          </p>
        </div>
        
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-lg mb-4">Quick Links</h4>
          <ul class="space-y-3 font-body text-sm text-[#888]">
            <li><a href="#home" class="hover:text-brand-green transition-colors">Home</a></li>
            <li><a href="#services" class="hover:text-brand-green transition-colors">Services</a></li>
            <li><a href="#projects" class="hover:text-brand-green transition-colors">Projects</a></li>
            <li><a href="#about" class="hover:text-brand-green transition-colors">About Us</a></li>
          </ul>
        </div>
        
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-lg mb-4">Services</h4>
          <ul class="space-y-3 font-body text-sm text-[#888]">
            <li><a href="#services" class="hover:text-brand-green transition-colors">Laser Cutting</a></li>
            <li><a href="#services" class="hover:text-brand-green transition-colors">Sheet Bending</a></li>
            <li><a href="#services" class="hover:text-brand-green transition-colors">Metal Structures</a></li>
            <li><a href="#services" class="hover:text-brand-green transition-colors">Custom Prototyping</a></li>
          </ul>
        </div>
        
        <div class="md:col-span-1">
          <h4 class="font-heading text-white text-lg mb-4">Legal</h4>
          <ul class="space-y-3 font-body text-sm text-[#888]">
            <li><a href="#" class="hover:text-brand-green transition-colors">Privacy Policy</a></li>
            <li><a href="#" class="hover:text-brand-green transition-colors">Terms of Service</a></li>
            <li><a href="#" class="hover:text-brand-green transition-colors">Sitemap</a></li>
          </ul>
        </div>
      </div>
      
      <div class="border-t border-[#222] pt-8 flex flex-col md:flex-row justify-between items-center">
        <p class="font-body text-[#555] text-xs uppercase tracking-widest mb-4 md:mb-0">
          &copy; {{ new Date().getFullYear() }} Metalúrgica Eblagon. All Rights Reserved.
        </p>
        <div class="flex gap-4">
          <!-- Social Icons Placeholder -->
          <a href="#" class="w-8 h-8 flex items-center justify-center bg-[#111] hover:bg-brand-green text-white transition-colors">in</a>
          <a href="#" class="w-8 h-8 flex items-center justify-center bg-[#111] hover:bg-brand-green text-white transition-colors">ig</a>
          <a href="#" class="w-8 h-8 flex items-center justify-center bg-[#111] hover:bg-brand-green text-white transition-colors">fb</a>
        </div>
      </div>
    </div>
  </footer>
</template>

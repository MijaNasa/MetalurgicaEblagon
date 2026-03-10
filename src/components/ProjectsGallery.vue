<script setup>
const projects = [
  { title: "Industrial Storage Racks", category: "Metal Structures" },
  { title: "Custom Laser Cut Panels", category: "Laser Cutting" },
  { title: "Agricultural Machinery Frames", category: "Industrial Fabrication" },
  { title: "Heavy Duty Conveyor system", category: "Assembly" },
  { title: "Stainless Steel Tanks", category: "Welding" },
  { title: "Folded Architectural Facade", category: "Sheet Bending" }
];
</script>

<template>
  <section id="projects" class="bg-[#0a0a0a] border-t border-[#111]">
    <div class="section-container">
      <div class="flex flex-col md:flex-row justify-between items-end mb-12">
        <div>
          <span class="font-body text-brand-green text-sm uppercase tracking-[0.2em] mb-2 block">Our Work</span>
          <h2 class="text-4xl md:text-5xl font-heading text-white border-b-4 border-brand-green inline-block pb-2">Recent Projects</h2>
        </div>
        <a href="#contact" class="hidden md:inline-block font-body text-brand-green hover:text-white uppercase tracking-wider text-sm mt-6 md:mt-0 transition-colors">Start Your Project →</a>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-1">
        <!-- Gallery Items -->
        <div 
          v-for="(item, index) in projects" 
          :key="index"
          class="group relative aspect-square overflow-hidden bg-[#111] cursor-pointer"
        >
          <!-- Placeholder background pattern for project image -->
          <div class="absolute inset-0 opacity-40 mix-blend-overlay bg-[linear-gradient(45deg,#222_25%,transparent_25%,transparent_75%,#222_75%,#222),linear-gradient(45deg,#222_25%,transparent_25%,transparent_75%,#222_75%,#222)] bg-[length:40px_40px] bg-[position:0_0,20px_20px]"></div>
          
          <div class="absolute inset-0 bg-brand-green/80 translate-y-full group-hover:translate-y-0 transition-transform duration-500 ease-in-out flex flex-col justify-end p-6">
            <span class="font-body text-white text-xs uppercase tracking-widest mb-2">{{ item.category }}</span>
            <h3 class="font-heading text-2xl text-black">{{ item.title }}</h3>
          </div>
        </div>
      </div>
      
      <div class="mt-8 text-center md:hidden">
        <a href="#contact" class="inline-block font-body text-brand-green hover:text-white uppercase tracking-wider text-sm transition-colors">Start Your Project →</a>
      </div>
    </div>
  </section>
</template>

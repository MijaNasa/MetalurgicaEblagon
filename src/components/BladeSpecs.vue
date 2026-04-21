<script setup>
const bladeModels = [
  {
    name: "Modelo 330 mm",
    specs: {
      diameter: "330 mm",
      cover: "270 mm",
      fixation: "57 mm",
      holes: 4
    },
    brands: ["Systel", "Pagani", "Marani", "Moretti", "Fadeco", "Freyre", "Bianchi", "Biserva", "Fiore", "Cibeles", "Platina", "El Sol", "San Salvador", "Trinidad"]
  },
  {
    name: "Modelo 300 mm (Opción A)",
    specs: {
      diameter: "300 mm",
      cover: "254 mm",
      fixation: "57 mm",
      holes: 4
    },
    brands: ["Freyre", "Trinidad"]
  },
  {
    name: "Modelo 300 mm (Opción B)",
    specs: {
      diameter: "300 mm",
      cover: "240 mm",
      fixation: "57 mm",
      holes: 4
    },
    brands: ["Marani", "Berkel", "San Salvador"]
  },
  {
    name: "Modelo 325 (Marani)",
    specs: {
      diameter: "325 mm",
      cover: "260 mm",
      fixation: "57 mm",
      holes: 4
    },
    brands: ["Marani"]
  }
];
</script>

<template>
  <section id="blade-specs" class="bg-[#080808] py-24">
    <div class="max-w-7xl mx-auto px-6">
      <!-- Header -->
      <div class="mb-16">
        <p class="font-body text-brand-green text-xs uppercase tracking-[0.3em] mb-4">Especificaciones Técnicas</p>
        <h2 class="font-heading text-white text-4xl md:text-6xl uppercase leading-[0.9]">
          MODELOS DE <span class="text-brand-green">CUCHILLAS</span>
        </h2>
      </div>

      <!-- Grid -->
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
        <div 
          v-for="(model, index) in bladeModels" 
          :key="index"
          class="group bg-white/5 border border-white/10 hover:border-brand-green/30 rounded-2xl p-8 transition-all duration-500"
        >
          <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-8 gap-4">
            <h3 class="font-heading text-white text-2xl uppercase group-hover:text-brand-green transition-colors">
              {{ model.name }}
            </h3>
            <div class="flex gap-2">
              <span class="px-3 py-1 bg-brand-green/10 border border-brand-green/20 rounded-full text-brand-green text-[10px] uppercase tracking-widest">
                Acero Inox
              </span>
              <span class="px-3 py-1 bg-white/5 border border-white/10 rounded-full text-white/40 text-[10px] uppercase tracking-widest">
                Precisión
              </span>
            </div>
          </div>

          <!-- Specs Table-like bits -->
          <div class="grid grid-cols-2 sm:grid-cols-4 gap-4 mb-8">
            <div class="bg-black/40 rounded-xl p-4 border border-white/5 group-hover:border-brand-green/10 transition-colors">
              <p class="text-white/30 text-[10px] uppercase tracking-wider mb-1">Diámetro</p>
              <p class="text-white font-heading text-lg">{{ model.specs.diameter }}</p>
            </div>
            <div class="bg-black/40 rounded-xl p-4 border border-white/5 group-hover:border-brand-green/10 transition-colors">
              <p class="text-white/30 text-[10px] uppercase tracking-wider mb-1">Cubre Cuchilla</p>
              <p class="text-white font-heading text-lg">{{ model.specs.cover }}</p>
            </div>
            <div class="bg-black/40 rounded-xl p-4 border border-white/5 group-hover:border-brand-green/10 transition-colors">
              <p class="text-white/30 text-[10px] uppercase tracking-wider mb-1">Fijación</p>
              <p class="text-white font-heading text-lg">Ø {{ model.specs.fixation }}</p>
            </div>
            <div class="bg-black/40 rounded-xl p-4 border border-white/5 group-hover:border-brand-green/10 transition-colors">
              <p class="text-white/30 text-[10px] uppercase tracking-wider mb-1">Agujeros</p>
              <p class="text-white font-heading text-lg">{{ model.specs.holes }}</p>
            </div>
          </div>

          <!-- Brands -->
          <div>
            <p class="text-white/30 text-[10px] uppercase tracking-widest mb-4">Marcas Compatibles</p>
            <div class="flex flex-wrap gap-2">
              <span 
                v-for="brand in model.brands" 
                :key="brand"
                class="px-3 py-1.5 bg-white/5 hover:bg-brand-green/20 border border-white/10 hover:border-brand-green/30 rounded-lg text-white/60 hover:text-white text-xs transition-all duration-300"
              >
                {{ brand }}
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Scoped styles if needed, but Tailwind is used */
</style>

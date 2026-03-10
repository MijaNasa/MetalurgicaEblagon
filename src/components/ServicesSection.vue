<script setup>
import ServiceCard from './ServiceCard.vue';

const services = [
  {
    title: 'Laser Cutting',
    description: 'High-precision CNC laser cutting for carbon steel, stainless steel, and aluminum sheets up to 20mm.',
    icon: '⚡' // Ideally replace with an SVG icon representing laser/cutting
  },
  {
    title: 'Sheet Metal Bending',
    description: 'Accurate bending and forming of metal components using automated press brakes with maximum tight tolerances.',
    icon: '📐' 
  },
  {
    title: 'Metal Structures',
    description: 'Heavy-duty steel frameworks and structural components for industrial buildings and warehouses.',
    icon: '🏗️'
  },
  {
    title: 'Custom Metal Parts',
    description: 'Prototyping and mass production of bespoke metal parts engineered strictly to your specifications.',
    icon: '⚙️'
  },
  {
    title: 'Industrial Fabrication',
    description: 'Complete assembly and welding services by certified professionals for complex industrial machinery.',
    icon: '🏭'
  },
  {
    title: 'Surface Finishing',
    description: 'Polishing, powder coating, and galvanizing to ensure durable protection against harsh environments.',
    icon: '✨'
  }
];
</script>

<template>
  <section id="services" class="bg-[#050505] relative border-t border-[#111]">
    <div class="section-container">
      <div class="text-center mb-16">
        <span class="font-body text-brand-green text-sm uppercase tracking-[0.2em] mb-2 block">Our Expertise</span>
        <h2 class="section-title">Industrial Services</h2>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <ServiceCard 
          v-for="(service, index) in services" 
          :key="index"
          :title="service.title"
          :description="service.description"
          :icon="service.icon"
        />
      </div>
    </div>
  </section>
</template>

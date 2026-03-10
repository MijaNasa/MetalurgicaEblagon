<template>
  <section id="process" class="bg-[#050505] border-t border-[#111]">
    <div class="section-container text-center">
      <span class="font-body text-brand-green text-sm uppercase tracking-[0.2em] mb-2 block">Workflow</span>
      <h2 class="section-title">Our Production Process</h2>
      
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mt-16 relative">
        <!-- Connecting Line -->
        <div class="hidden lg:block absolute top-[40px] left-[10%] w-[80%] h-1 bg-[#222]"></div>
        
        <!-- Step 1 -->
        <div class="relative z-10 group">
          <div class="w-20 h-20 mx-auto bg-black border-2 border-brand-gray text-brand-gray rounded-full flex items-center justify-center font-heading text-3xl mb-6 transition-colors duration-300 group-hover:border-brand-green group-hover:bg-brand-green group-hover:text-black">
            1
          </div>
          <h4 class="text-xl font-heading text-white mb-2">Request Quote</h4>
          <p class="font-body text-sm text-brand-gray">Submit your technical drawings and requirements to our engineering team.</p>
        </div>
        
        <!-- Step 2 -->
        <div class="relative z-10 group">
          <div class="w-20 h-20 mx-auto bg-black border-2 border-brand-gray text-brand-gray rounded-full flex items-center justify-center font-heading text-3xl mb-6 transition-colors duration-300 group-hover:border-brand-green group-hover:bg-brand-green group-hover:text-black">
            2
          </div>
          <h4 class="text-xl font-heading text-white mb-2">Technical Review</h4>
          <p class="font-body text-sm text-brand-gray">Our experts analyze tolerances, materials, and optimize the production process.</p>
        </div>
        
        <!-- Step 3 -->
        <div class="relative z-10 group">
          <div class="w-20 h-20 mx-auto bg-black border-2 border-brand-gray text-brand-gray rounded-full flex items-center justify-center font-heading text-3xl mb-6 transition-colors duration-300 group-hover:border-brand-green group-hover:bg-brand-green group-hover:text-black">
            3
          </div>
          <h4 class="text-xl font-heading text-white mb-2">Fabrication</h4>
          <p class="font-body text-sm text-brand-gray">Your order is manufactured swiftly on our advanced CNC machines and welding spots.</p>
        </div>
        
        <!-- Step 4 -->
        <div class="relative z-10 group">
          <div class="w-20 h-20 mx-auto bg-black border-2 border-brand-gray text-brand-gray rounded-full flex items-center justify-center font-heading text-3xl mb-6 transition-colors duration-300 group-hover:border-brand-green group-hover:bg-brand-green group-hover:text-black">
            4
          </div>
          <h4 class="text-xl font-heading text-white mb-2">Delivery</h4>
          <p class="font-body text-sm text-brand-gray">Final quality assurance checks and logistical shipment directly to your site.</p>
        </div>
        
      </div>
    </div>
  </section>
</template>

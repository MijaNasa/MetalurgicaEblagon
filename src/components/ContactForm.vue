<script setup>
import { ref } from 'vue';

const form = ref({
  name: '',
  company: '',
  email: '',
  phone: '',
  message: ''
});

const handleSubmit = (e) => {
  e.preventDefault();
  // Design only, no backend needed
  alert('Thank you for your message. We will contact you shortly.');
  form.value = { name: '', company: '', email: '', phone: '', message: '' };
};
</script>

<template>
  <section id="contact" class="bg-[#0a0a0a] border-t border-[#111]">
    <div class="section-container">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
        <div>
          <span class="font-body text-brand-green text-sm uppercase tracking-[0.2em] mb-2 block">Get in Touch</span>
          <h2 class="text-4xl md:text-5xl font-heading mb-8 text-white">Start Your Project</h2>
          <p class="font-body text-brand-gray mb-10 leading-relaxed text-lg">
            Ready to manufacture with precision? Send us your project details or call us directly. Our engineering team is standing by to provide a comprehensive technical review and competitive quote.
          </p>
          
          <div class="space-y-6 mb-12">
            <div class="flex items-center text-brand-gray">
              <span class="text-brand-green mr-4 text-xl">📍</span>
              <span class="font-body text-sm uppercase tracking-wider">Córdoba, Argentina</span>
            </div>
            <div class="flex items-center text-brand-gray">
              <span class="text-brand-green mr-4 text-xl">📞</span>
              <span class="font-body text-sm">+54 351 123 4567</span>
            </div>
            <div class="flex items-center text-brand-gray">
              <span class="text-brand-green mr-4 text-xl">✉️</span>
              <span class="font-body text-sm">quotes@metalurgicaeblagon.com</span>
            </div>
          </div>
          
          <!-- WhatsApp Button -->
          <a href="https://wa.me/543511234567" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-3 bg-[#25D366] hover:bg-[#128C7E] text-white font-body px-6 py-4 rounded font-bold uppercase tracking-wider transition-colors w-full sm:w-auto justify-center shadow-[0_4px_20px_rgba(37,211,102,0.3)]">
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current" xmlns="http://www.w3.org/2000/svg"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51a12.8 12.8 0 0 0-.57-.01c-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 0 1-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 0 1-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 0 1 2.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0 0 12.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 0 0 5.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 0 0-3.48-8.413Z"/></svg>
            WhatsApp Direct
          </a>
        </div>
        
        <div>
          <form @submit="handleSubmit" class="bg-[#111] border border-[#222] p-8">
            <h3 class="font-heading text-2xl text-white mb-6">Request Quote</h3>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-6">
              <div>
                <label for="name" class="block font-body text-xs text-brand-gray uppercase tracking-widest mb-2">Full Name</label>
                <input type="text" id="name" v-model="form.name" required class="w-full bg-black border border-[#333] text-white p-3 font-body focus:border-brand-green focus:outline-none transition-colors">
              </div>
              <div>
                <label for="company" class="block font-body text-xs text-brand-gray uppercase tracking-widest mb-2">Company</label>
                <input type="text" id="company" v-model="form.company" class="w-full bg-black border border-[#333] text-white p-3 font-body focus:border-brand-green focus:outline-none transition-colors">
              </div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-6">
              <div>
                <label for="email" class="block font-body text-xs text-brand-gray uppercase tracking-widest mb-2">Email Address</label>
                <input type="email" id="email" v-model="form.email" required class="w-full bg-black border border-[#333] text-white p-3 font-body focus:border-brand-green focus:outline-none transition-colors">
              </div>
              <div>
                <label for="phone" class="block font-body text-xs text-brand-gray uppercase tracking-widest mb-2">Phone Number</label>
                <input type="tel" id="phone" v-model="form.phone" required class="w-full bg-black border border-[#333] text-white p-3 font-body focus:border-brand-green focus:outline-none transition-colors">
              </div>
            </div>
            
            <div class="mb-8">
              <label for="message" class="block font-body text-xs text-brand-gray uppercase tracking-widest mb-2">Project Details & Message</label>
              <textarea id="message" v-model="form.message" rows="4" required class="w-full bg-black border border-[#333] text-white p-3 font-body focus:border-brand-green focus:outline-none transition-colors resize-none"></textarea>
            </div>
            
            <button type="submit" class="w-full btn-primary py-4 hover:shadow-[0_4px_30px_rgba(29,94,65,0.4)]">
              Send Specification
            </button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

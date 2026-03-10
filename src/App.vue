<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
import ServicesSection from './components/ServicesSection.vue';
import WhyChooseUs from './components/WhyChooseUs.vue';
import ProcessSection from './components/ProcessSection.vue';
import ProjectsGallery from './components/ProjectsGallery.vue';
import AboutSection from './components/AboutSection.vue';
import ContactForm from './components/ContactForm.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <div class="bg-black min-h-screen text-white overflow-x-hidden selection:bg-brand-green selection:text-white">
    <!-- Main Navigation -->
    <Navbar />
    
    <main>
      <!-- Hero / Landing Area -->
      <HeroSection />
      
      <!-- Core Services List -->
      <ServicesSection />
      
      <!-- Value Proposition / Advantages -->
      <WhyChooseUs />
      
      <!-- Step-by-Step Workflow -->
      <ProcessSection />
      
      <!-- Portfolio Grid -->
      <ProjectsGallery />
      
      <!-- Company Information -->
      <AboutSection />
      
      <!-- Contact Information & Form -->
      <ContactForm />
    </main>
    
    <!-- Site Footer -->
    <Footer />
  </div>
</template>

<style>
/* Any additional global fixes */
* {
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
  width: 100%;
}
</style>

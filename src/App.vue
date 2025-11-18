<template>
  <div class="bg-[#0F172A] min-h-screen overflow-x-hidden">
    <Navbar/>
    <Accueil/>
    <Present/> 
    <Portfolio/>
    <Competence/>
    <Contact/>
    <Footer/>
  </div>
</template>

<script setup>
  import { defineAsyncComponent } from 'vue';

  const Navbar = defineAsyncComponent(()=>import('@/components/layout/Navbar.vue'))
  const Accueil = defineAsyncComponent(()=>import('@/components/layout/Accueil.vue'))
  const Present = defineAsyncComponent(()=>import('@/components/layout/Present.vue'))
  const Portfolio = defineAsyncComponent(()=>import('@/components/layout/Portfolio.vue'))
  const Competence = defineAsyncComponent(()=>import('@/components/layout/Competence.vue'))
  const Contact = defineAsyncComponent(()=>import('@/components/layout/Contact.vue'))
  const Footer = defineAsyncComponent(()=>import('@/components/layout/Footer.vue'))
</script>

<template>
  <div class="bg-[#0F172A] min-h-screen">
    <Navbar/>
    <Accueil/>
     <Present/> 
  </div>
</template>

<script setup>
  import { defineAsyncComponent } from 'vue';

  const Navbar = defineAsyncComponent(()=>import('@/components/layout/Navbar.vue'))
  const Accueil = defineAsyncComponent(()=>import('@/components/layout/Accueil.vue'))
  const Present = defineAsyncComponent(()=>import('@/components/layout/Present.vue'))
</script>


<template>
  <div class="bg-[#0F172A] min-h-screen">
    <Navbar/>
  </div>
</template>

<script setup>
  import { defineAsyncComponent } from 'vue';

  const Navbar = defineAsyncComponent(()=>import('@/components/navbar.vue'))
</script>


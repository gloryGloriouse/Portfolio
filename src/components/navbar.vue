<template>
    <header>
        <div class="flex justify-between items-center p-6 lg:px-12 relative z-20">
            <div class="text-3xl font-bold dark:text-white">PortFolio</div>    
            <!--Button du menu-->
            <div class="md:hidden z-30" @click="isMenuOpen = !isMenuOpen ">
                <button class="block focus:outline-none">
                    <span v-if="isMenuOpen" class="text-5xl md:text-[#A3CCDA] text-white">
                        <Icon icon="material-symbols:close"/>
                    </span>
                    <span v-else class="text-5xl md:text-[#A3CCDA] text-white">
                        <Icon icon="material-symbols:menu"/>
                    </span>
                </button>
            </div>
            <!--lien du nav-->
            <nav :class="[
                    'fixed inset-0 flex flex-col items-center justify-center bg-[#A3CCDA] transition-all duration-500 ease-in-out',
                    isMenuOpen ? 'opacity-100 translate-y-0 pointer-events-auto' : 'opacity-0 -translate-y-10 pointer-events-none',
                    'md:relative md:flex md:flex-row md:justify-between md:bg-transparent md:opacity-100 md:translate-y-0 md:pointer-events-auto'
                ]">
                <ul class="flex flex-col items-center space-y-5 md:flex-row md:space-x-5 md:space-y-0">
                    <li v-for="item in Menu" :key="item.name">
                        <a :href="item.href" class="block transtion ease-linear md:text-lg lg:text-2xl
                        font-semibold text-white  hover:text-blue-300 text-2xl" 
                        @click="scrollToSection(item.href)">{{ item.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)
const Menu = ref([
    {name:'Accueil',href:'#accueil'},
    {name:'Services',href:'#services'},
    {name:'Compétence',href:'#compétence'},
    {name:'Projets',href:'#projets'},
    {name:'Me Contacte',href:'#contact'},
])

const scrollToSection = (href) => {
    isMenuOpen.value = false;
    const section = document.querySelector(href);
    if(section){
        section.scrollIntoView({behavior:'smooth'})
    }
}
</script>

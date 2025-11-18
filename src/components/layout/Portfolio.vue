<template>
    <div data-aos="fade-up" id="portfolio" class="w-full text-white p-6 lg:p-12 ">
        <Title title="Projets"/>
        <div class="max-w-6xl mx-auto grid grid-cols-1 sm:grid-cols-2  lg:grid-cols-3 gap-12 items-center justify-items-center">
            <article v-for="projet in projet" :key="projet.title" 
            class="w-[300px] h-[380px] mx-auto flex flex-col overflow-hidden rounded-xl shadow-lg border border-[#06b6d4] 
            bg-white/10 backdrop-blur-sm transition-transform duration-300 hover:-translate-y-2">
              <!-- Image -->
                <figure class="w-full h-44 overflow-hidden">
                    <img :src="projet.image" class="w-full h-full object-cover object-center">
                </figure>
                <!-- Content -->
                <div class="flex-1 p-5 flex flex-col">
                    <h3 class="font-semibold text-xl text-white mb-2">
                    {{ projet.title }}
                    </h3>
                    <!-- Description limitée automatiquement -->
                    <p class="text-sm text-slate-300/80 line-clamp-3">
                    {{ projet.Description }}
                    </p>
                </div>
                <!-- Button -->
                <div class="pb-4 flex justify-center">
                    <a :href="projet.LiveLink"
                    class="bg-[#06b6d4] text-white px-4 py-2 rounded-full border border-[#06b6d4] hover:text-[#06b6d4] hover:bg-transparent hover:bg-[#06b6d4]/80 transition">
                    Voir le projet
                    </a>
                </div>
            </article>
        </div>
    </div>
</template>
<script setup>
 import Title from '@/components/UI/title.vue'
 import logoResto from '@/assets/logoResto.jpg'
 import Rocket from '@/assets/rocket.png'
 import digital from '@/assets/d3.jpg'
 import Flex from '@/assets/flex.jpg'
 import Console from '@/assets/console.jpg'

 const projet = [
  { image:logoResto, title: 'Restaurant', Description: 'siteweb responsive de restaurant.', tags: 'HTML, CSS, JavaScript', LiveLink: '/projet/Resto/html.html'},
  { image:digital, title: 'Agence digital', Description:'siteweb responsive d\'une agence digital .', tags: 'HTML, CSS, JavaScript', LiveLink: '/projet/digital/index.html'},
  { image:Rocket, title: 'Astro world', Description: 'siteweb responsive d\'astronaut', tags: 'HTML, Tailwindcss', LiveLink: 'https://glo-rockets.onrender.com'},
  { image:Flex, title: 'Social Help', Description:'Plateforme de placement de menageres et AVS.', tags: 'HTML, CSS, JavaScript', LiveLink: 'https://github.com/audreyvilleneuve/restaurant'},
  //{ image:Console, title: 'PHP', Description:'siteweb responsive de restaurant.', tags: 'HTML, CSS, JavaScript', LiveLink: 'https://github.com/audreyvilleneuve/restaurant'},
  //{ image:logoResto, title: 'Leave Mangement', Description:'Site de gestion de personnelle d\'une Entreprise.', tags: 'HTML, CSS, JavaScript', LiveLink: 'https://github.com/audreyvilleneuve/restaurant'}, 
]
</script>

<template>
    <div data-aos="fade-up" id="competence" class="w-full text-white p-6 lg:p-12">
        <Title title="Compétences"/>
        <div class="max-w-6xl mx-auto grid lg:grid-cols-2 gap-6" data-aos="fade-up">
            <div v-for="skill in skills" :key="skill.name"
              class="rounded-xl border border-[#06b6d4]/60 bg-white/5 p-4 overflow-hidden ">
                <div class="flex items-center justify-between mb-2 text-sm">
                    <span class="font-semibold text-slate-200">{{ skill.name }}</span>
                    <span class="text-slate-300">{{ skill.level }}%</span>
                </div>
                <div class="w-full h-3 rounded-xl bg-white/15 overflow-hidden">
                    <div class="h-full bg-[#06b6d4] rounded-xl transition-all duration-700 ease-out"
                    :style="{ width: skill.level + '%' }" />
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import Title from '@/components/UI/title.vue'
const skills = [
  { name: 'HTML', level: 90 },
  { name: 'CSS', level: 85 },
  { name: 'JavaScript', level: 50 },
  { name: 'PHP', level: 70 },
  { name: 'TailwindCSS', level: 65 },
  { name: 'Vue.js', level: 40 },
  { name: 'Laravel', level: 40 }
]
</script>

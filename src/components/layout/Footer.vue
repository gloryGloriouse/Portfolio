<template>
  <footer class="text-white border-t border-white/10 bg-white/5 backdrop-blur-sm ">
    <div class="max-w-6xl mx-auto p-2 h-full flex flex-col md:flex-row items-center justify-between gap-4">
      <div class="text-sm text-slate-300">
        {{ year }} Audrey Glory. Tous droits réservés.
      </div>

      <nav class="flex items-center gap-4 text-sm">
        <a href="#presentation" @click.prevent="scrollTo('#presentation')" class="hover:text-cyan-400 transition-colors">Présentation</a>
        <a href="#portfolio" @click.prevent="scrollTo('#portfolio')" class="hover:text-cyan-400 transition-colors">Projets</a>
        <a href="#competence" @click.prevent="scrollTo('#competence')" class="hover:text-cyan-400 transition-colors">Compétences</a>
      </nav>

      <div class="flex items-center gap-3">
        <a href="#nav" aria-label="Haut de page" @click.prevent="scrollToNav" class="p-2 rounded-full border border-white/20 text-white hover:border-[#06b6d4] text-slate-200 hover:text-[#06b6d4] transition-colors">
          <Icon icon="mdi:arrow-up" class="text-xl" />
        </a>
      </div>
    </div>
  </footer>
</template>

<script setup>
const year = new Date().getFullYear()

const scrollTo = (href) => {
  const el = document.querySelector(href)
  if (el) el.scrollIntoView({ behavior: 'smooth', block: 'start' })
}

const scrollToNav = () => {
  const el = document.getElementById('nav')
  if (el) el.scrollIntoView({ behavior: 'smooth', block: 'start' })
}
</script>



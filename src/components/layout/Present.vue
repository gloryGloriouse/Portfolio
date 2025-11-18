<template>
  <section id="presentation" data-aos="fade-up" class="w-full text-white py-6 lg:py-12 scroll-mt-24">
    <div class="group flex flex-col py-8 items-center">
        <h2 class="text-3xl lg:text-4xl font-bold transition-all duration-300 text-center head " data-aos="fade-up" >Présentation</h2>
        <div class="w-24 h-1  mx-auto mt-2 transition-all duration-300 rounded-full group-hover:bg-cyan-500/70"></div>
    </div>
    <div class="max-w-6xl mx-auto px-4 lg:px-8 grid lg:grid-cols-2 gap-12 items-center rounded-xl border border-white/10 bg-white/5 backdrop-blur-sm p-6 flex flex-col items-start gap-2">
        <div class="space-y-6">
            <div class="group flex flex-col py-8 items-center" data-aos="fade-up">
                <h2 class="text-2xl lg:text-3xl font-semibold text-center text-[#06b6d4] head transition-all duration-300" data-aos="fade-up" >Audrey Glory .T.</h2>
                <div class="w-24 h-1  mx-auto mt-2  rounded-full bg-cyan-500/70"></div>
            </div>
          <p data-aos="fade-up">
            Développeuse Web passionnée par la création d’expériences modernes, performantes et accessibles.
            J’aime transformer des idées en interfaces élégantes et des solutions robustes, avec une attention
            particulière portée à la performance, la sécurité et l’UX.
          </p>
          <ul class="mt-4 space-y-3" data-aos="fade-up" data-aos-delay="100">
            <li class="flex items-start gap-2 text-slate-300">
              <Icon icon="mdi:map-marker" class="text-cyan-400 text-xl mt-0.5" />
              <span><span class="text-slate-200 font-medium">Basée à</span>: Douala, Cameroun</span>
            </li>
            <li class="flex items-start gap-2 text-slate-300">
              <Icon icon="mdi:briefcase-clock" class="text-cyan-400 text-xl mt-0.5" />
              <span><span class="text-slate-200 font-medium">Disponibilité</span>: freelance & projets à temps partiel</span>
            </li>
            <li class="flex items-start gap-2 text-slate-300">
              <Icon icon="mdi:translate" class="text-cyan-400 text-xl mt-0.5" />
              <span><span class="text-slate-200 font-medium">Langues</span>: Français, Anglais</span>
            </li>
          </ul>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 ">
            <h2 class="col-span-1 sm:col-span-2 text-xl lg:text-2xl font-bold text-center text-[#06b6d4]" data-aos="fade-up">Services</h2>

            <div class="rounded-xl border border-white/10 bg-white/5 p-5 transition-transform duration-300 hover:-translate-y-1 hover:bg-white/10" data-aos="fade-up" >
              <div class="flex items-start gap-3">
                <Icon icon="mdi:web" class="text-cyan-400 text-2xl" />
                <div>
                  <h4 class="font-semibold">Front‑end</h4>
                  <p class="text-sm text-slate-300/80">Interfaces modernes, réactives et accessibles.</p>
                </div>
              </div>
            </div>

            <div class="rounded-xl border border-white/10 bg-white/5 p-5 transition-transform duration-300 hover:-translate-y-1 hover:bg-white/10" data-aos="fade-up" >
              <div class="flex items-start gap-3">
                <Icon icon="mdi:code-tags" class="text-cyan-400 text-2xl" />
                <div>
                  <h4 class="font-semibold">Back‑end</h4>
                  <p class="text-sm text-slate-300/80">APIs sécurisées et logiques robustes.</p>
                </div>
              </div>
            </div>

            <div class="rounded-xl border border-white/10 bg-white/5 p-5 transition-transform duration-300 hover:-translate-y-1 hover:bg-white/10" data-aos="fade-up" >
              <div class="flex items-start gap-3">
                <Icon icon="mdi:api" class="text-cyan-400 text-2xl" />
                <div>
                  <h4 class="font-semibold">Intégration API</h4>
                  <p class="text-sm text-slate-300/80">Connexion de services tiers et automatisations.</p>
                </div>
              </div>
            </div>

            <div class="rounded-xl border border-white/10 bg-white/5 p-5 transition-transform duration-300 hover:-translate-y-1 hover:bg-white/10" data-aos="fade-up" >
              <div class="flex items-start gap-3">
                <Icon icon="mdi:brush" class="text-cyan-400 text-2xl" />
                <div>
                  <h4 class="font-semibold">UI/UX & Tailwind</h4>
                  <p class="text-sm text-slate-300/80">Design cohérent et optimisé pour l’expérience.</p>
                </div>
              </div>
            </div>
        </div>
      </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.head:hover{
    color: transparent;
    -webkit-text-stroke-width: 2px;
    -webkit-text-stroke-color: #06b6d4;
}
</style>
<template>
    <div
    data-aos="fade-up" id="accueil"
    class="flex  min-h-[calc(100vh-6rem)]  justify-center lg:justify-start items-center text-white lg:mt-0">
        <main class="flex flex-col lg:grid lg:!grid-cols-2 w-full  mx-auto items-center lg:px-8 ">
            <div class="text-center lg:!text-left px-2 lg:px-0 order-2 lg:order-1">

                <h1 class="mb-6 text-2xl lg:text-4xl font-bold">
                    Salut, je suis <span class="text-stroke text-stroke-cyan text-3xl lg:text-5xl">Audrey Glory</span>
                </h1>
                <h1 class="mb-4 text-xl lg:text-2xl font-bold">
                    Je suis  <span class="text-[#06b6d4]">Développeuse Web</span>
                </h1>
                <p class="text-lg mx-auto max-w-xl lg:mx-0 ">
                    Je crée des sites web modernes et performants, en développement Front-end et Back-end.
                    Chaque projet est l'occasion d'allier efficacité et élégance, avec une attention particulière portée à la performance, la sécurité et l'expérience utilisateur. Passionné par l'apprentissage continu, 
                    je transforme les idées en solutions concrètes et fonctionnelles.
                </p>
                <div class="mt-6 flex flex-col sm:flex-row flex-wrap justify-center sm:justify-start items-center gap-y-4 sm:gap-y-0 gap-x-6 lg:gap-x-24">
                    <button class="bg-[#06b6d4] font-semibold text-white px-6 py-2 rounded-full mt-6 hover:!bg-transparent hover:!text-[#06b6d4] border-2 border-[#06b6d4] 
                        transition-all duration-300 flex items-center gap-2">
                        Télécharger CV
                        <Icon icon="line-md:download-loop" class="text-xl" />
                    </button>
                    <div class="flex gap-4 mt-6">
                        <!-- WhatsApp -->
                        <a href="#" class="p-2 rounded-full bg-[#06b6d4] text-white border-1 border-[#06b6d4] 
                            hover:!bg-transparent hover:!text-[#06b6d4] transition-all duration-300">
                            <Icon icon="mdi:whatsapp" class="text-2xl" />
                        </a>
                        <!-- Facebook -->
                        <a href="#" class="p-2 rounded-full bg-[#06b6d4] text-white border-1 border-[#06b6d4] 
                            hover:!bg-transparent hover:!text-[#06b6d4] transition-all duration-300">
                            <Icon icon="mdi:facebook" class="text-2xl" />
                        </a>
                        <!-- LinkedIn -->
                        <a href="#" class="p-2 rounded-full bg-[#06b6d4] text-white border-1 border-[#06b6d4] 
                            hover:!bg-transparent hover:!text-[#06b6d4] transition-all duration-300">
                            <Icon icon="mdi:linkedin" class="text-2xl" />
                        </a>

                        <!-- YouTube -->
                        <a href="#" class="p-2 rounded-full bg-[#06b6d4] text-white border-1 border-[#06b6d4] 
                            hover:!bg-transparent hover:!text-[#06b6d4] transition-all duration-300">
                            <Icon icon="mdi:youtube" class="text-2xl" />
                        </a>
                    </div>
                </div>
            </div>

      <!-- Image avec effet wavy -->
      <div class="flex justify-center items-center order-1 lg:order-2">

        <div class="container">
          <figure class="card">
            <div class="image-wrapper">
              <img 
                src="@/assets/Audrey1.jpg" 
                alt="Audrey Glory" 
                class="profile-image"
              />
            </div>
          </figure>
        </div>
      </div>
    </main>

    <!-- SVG pour effet wavy -->
    <svg class="hidden">
      <defs>
        <filter id="wavy1">
          <feTurbulence type="fractalNoise" baseFrequency="0.015" numOctaves="3" seed="2" result="turb">
            <animate attributeName="baseFrequency" dur="10s" values="0.015;0.025;0.015" repeatCount="indefinite" />
          </feTurbulence>
          <feDisplacementMap in="SourceGraphic" in2="turb" scale="15" />
        </filter>
      </defs>
    </svg>
  </div>
</template>

<script setup>
</script>

<style>
.text-stroke {
  color: transparent;
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #06b6d4;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

.container .card {
  position: relative;
  width: clamp(260px, 70vw, 420px);
  height: clamp(260px, 70vw, 420px);
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Effet contour wavy CARRÉ avec pseudo-élément */
.container .card::before {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  border: 8px solid #06b6d4;
  border-radius: 20px; /* Coins légèrement arrondis pour un carré moderne */
  box-shadow: 0 0 25px #06b6d4, 0 0 50px rgba(6, 182, 212, 0.5);
  z-index: 1;
  background: transparent;
  filter: url(#wavy1); /* L'effet wavy sur le contour CARRÉ */
}

.image-wrapper {
  position: relative;
  width: calc(100% - 40px);
  height: calc(100% - 40px);
  z-index: 2;
}

.profile-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 15px; /* Coins arrondis assortis au contour */
  border: 4px solid #06b6d4;
}
</style>
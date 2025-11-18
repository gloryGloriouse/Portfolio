<template>
    <div data-aos="fade-up" id="contact" class="w-full text-white p-6 lg:p-12  min-h-[calc(100vh-6rem)]">
        <Title title="Me Contacte"/>
        <div class="max-w-6xl mx-auto grid gap-4 items-center " data-aos="fade-up" >
            <input type="text" placeholder="Nom" data-aos="fade-up" class="w-full p-2 rounded-xl border border-[#06b6d4] bg-white/5 transition-transform duration-300 hover:-translate-y-2 hover:bg-white/15" />
            <input type="text" placeholder="Email" data-aos="fade-up" class="w-full p-2 rounded-xl border border-[#06b6d4] bg-white/5 transition-transform duration-300 hover:-translate-y-2 hover:bg-white/15" />
            <textarea cols="25" rows="10" placeholder="Message" data-aos="fade-up" class="w-full p-2 rounded-xl border border-[#06b6d4] bg-white/5 transition-transform duration-300 hover:-translate-y-2 hover:bg-white/15"></textarea>
            <div>
                <button class="bg-[#06b6d4] font-semibold text-white px-6 py-2 rounded-full hover:!bg-transparent hover:!text-[#06b6d4] ring-[#06b6d4] ring-2 
                    transition-all duration-300 cursor-pointer">
                    Envoyer
                </button>
            </div>
        </div>
    </div>
    
</template>
<script setup>
import Title from '@/components/UI/title.vue'
</script>
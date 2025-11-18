<template>
    <div class="group flex flex-col py-6 items-center">
        <h2 class="text-3xl lg:text-4xl font-bold transition-all duration-300 text-center text-stroke text-stroke-cyan " data-aos="fade-up" > <slot>{{ props.title }}</slot></h2>
        <div class="w-24 h-1 mx-auto mt-2 transition-all duration-300 rounded-full group-hover:bg-cyan-500/70 hover:shadow-cyan-500/70"></div>
    </div>
</template>
<script setup>
    const props = defineProps({
        title: {
            type: String,
            required: true
        }
    })
</script>
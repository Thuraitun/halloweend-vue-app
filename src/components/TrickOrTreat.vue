<template>
    <section id="trickortreat" class="flex flex-col items-center py-28">
        <h2 class="mt-10 text-6xl font-bold text-center text-white mb-28">Trick Or Treat </h2>
        <div class="grid grid-cols-1 gap-10 md:grid-cols-3">
            <div 
                v-for="(item,i) in items" 
                :key="item.title" 
                class="grid gap-5 p-8 text-center text-white rounded-md bg-gradient-to-br place-items-center"
                :class="i === 1 ? 
                'md:from-primary-200/80 md:to-primary-2 00/30 md:-translate-y-16 ' 
                : 'from-primary-200/20 to-primary-200/10'"
            >
                <div class="">
                    <img :src="item.image" alt="">
                </div>
                <h3 class="text-2xl font-bold ">{{ item.title }}</h3>
                <p class=" w-[80%]">{{ item.desc }}</p>
            </div>
        </div>
    </section>
</template>

<script setup>
    import items from "../data/trickortreat";
</script>

<style scoped></style>
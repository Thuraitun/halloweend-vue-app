<template>
    <section id="category" class="flex flex-col items-center pt-20">
        <h1 class="my-12 text-5xl font-bold text-white">Category</h1>
        <div class="grid grid-cols-3 place-items-center">
            <div v-for="category in categories" :key="category.title" class="grid text-center text-white place-items-center">
                <div class="p-10">
                    <img :src="category.image" alt="">
                </div>
                <h1 class="text-3xl font-bold">{{category.title}}</h1>
                <p class="w-3/4">{{category.desc}} </p>
            </div>
        </div>
    </section>
    <section class="grid items-center grid-flow-col grid-cols-2 gap-10 mt-20">
        <div class="items-start p-10 bg-green-500">
            <img src="../assets/image/category2-img.webp" alt="">
        </div>
        <div class="bg-yellow-500">
            <div class="text-6xl font-bold text-white">
                <h2 class="mb-5">What's that</h2>
                <div class="flex gap-5"> 
                    <h2 class="">Halloweend</h2>
                    <img src="../assets/image/head2-img.png" alt="">
                </div>
            </div>
            <p class="w-[80%] mt-10 text-xl text-white">Halloween or Hallowe'en, also known as Allhalloween, All Hallows' Eve, or All Saints' Eve, is a celebration observed in many countries on 31 October, the eve of the Western Christian feast of All Hallows' Day.</p>
        </div>
    </section>
</template>

<script setup>
    import category1 from "../assets/image/category/category1-img.webp";
    import category2 from "../assets/image/category/category2-img.webp";
    import category3 from "../assets/image/category/category3-img.webp";

    const categories = [
        {
            title: 'Ghost',
            image: category1,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
        },
        {
            title: 'Witch',
            image: category2,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
        },
        {
            title: 'Pumpkin',
            image: category3,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
        },
    ]
</script>

<style scoped>

</style>
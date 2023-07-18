<template>
    <section id="category" class="">
        <div class="py-24 ">
            <h3 class="text-6xl font-bold text-center text-white mb-14">Category</h3>
            <div class="flex flex-col md:space-x-24 md:flex-row">
                <div class="" v-for="category in categories" :key="category.title">
                    <div class="flex flex-col items-center justify-center text-white">
                        <img :src="category.image" alt="" class="">
                        <p class="text-3xl ">{{ category.title }}</p>
                        <p class="w-2/3 text-center">{{ category.desc }}</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- about -->
        <div id="about" class="flex flex-col items-center justify-center md:flex-row">
            <div class="w-full md:w-1/2 ">
                <img src="../assets/image/category2-img.webp" alt="">
            </div>
            <div class="flex flex-col items-center justify-center px-8 md:w-1/2 md:ps-32 md:justify-start md:items-start">
                <div class="text-3xl font-bold text-white md:text-6xl">
                    <h1 class="mb-4">What's that</h1>
                    <div class="flex space-x-3">
                        <h1 class="">Halloween</h1>
                        <img src="../assets/image/head2-img.png" alt="">
                    </div>
                </div>
                <p class="text-center text-white md:text-xl md:text-left">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod sapiente soluta voluptates saepe officia nulla, ab ad, quae, rerum id magnam </p>
            </div>
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
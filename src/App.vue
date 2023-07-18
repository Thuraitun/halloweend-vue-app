<template>
  <div class="container">
    <Navbar />
    <Home />
    <Category />
    <TrickOrTreat />
    <Subscribe />
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue';
import Category from './components/Categroy.vue'
import TrickOrTreat from './components/TrickOrTreat.vue'
import Subscribe from './components/Subscribe.vue'
import Footer from './components/Footer.vue'
</script>

<style scoped></style>
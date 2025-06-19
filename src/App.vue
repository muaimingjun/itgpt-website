<template>
  <Header />
  <main>
    <Hero />
    <Features />
  </main>
  <Footer />
</template>

<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Features from './components/Features.vue'
import Footer from './components/Footer.vue'
</script>

<style>
/* All global styles are now in src/assets/main.css and src/assets/base.css */
/* This keeps App.vue clean and focused on layout structure. */
</style>

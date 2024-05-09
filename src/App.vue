<script setup>
import TheWelcome from '@/components/TheWelcome.vue'
import Navbar from '@/components/Navbar.vue'
import Aboutme from './components/Aboutme.vue'
import Plan from './components/Plan.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <header>
    <Navbar />
    <TheWelcome />
    <Aboutme />
    <Plan />
    <Footer />
  </header>
</template>

<style scoped></style>

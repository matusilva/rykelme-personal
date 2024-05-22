<script setup>
import Navbar from '@/components/Navbar.vue'
import TheWelcome from '@/components/TheWelcome.vue'
import HowItWorks from './components/HowItWorks.vue'
import BeforeAfter from './components/BeforeAfter.vue'
import Aboutme from './components/Aboutme.vue'
import Plan from './components/Plan.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <header>
    <Navbar />
    <TheWelcome />
    <HowItWorks />
    <BeforeAfter />
    <Plan />
    <Aboutme />
    <Footer />
  </header>
</template>

<style scoped></style>

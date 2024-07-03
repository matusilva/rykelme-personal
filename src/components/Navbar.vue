<script setup>
import { ref } from 'vue'

const isOpen = ref(false)

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}
</script>

<template>
  <nav
    class="relative bg-gray-800 bg-cover"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)),
        url(/background.jpeg);
    "
  >
    <div class="container mx-auto px-6 py-4 md:flex md:items-center md:justify-between">
      <div class="flex items-center justify-between">
        <a href="#">
          <img class="h-14 w-auto" src="/logo/logo.png" alt="" />
        </a>
        <div class="flex md:hidden">
          <button
            @click="toggleMenu"
            type="button"
            class="text-gray-200 hover:text-gray-400 focus:text-gray-400 focus:outline-none"
            aria-label="toggle menu"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              :class="{ hidden: isOpen, block: !isOpen }"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path stroke-linecap="round" stroke-linejoin="round" d="M4 8h16M4 16h16" />
            </svg>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              :class="{ hidden: !isOpen, block: isOpen }"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
      </div>
      <div
        :class="{ block: isOpen, hidden: !isOpen }"
        class="absolute inset-x-0 z-20 w-full bg-black px-6 py-4 opacity-95 transition-all duration-300 ease-in-out md:relative md:top-0 md:mt-0 md:flex md:w-auto md:translate-x-0 md:items-center md:bg-transparent md:p-0 md:opacity-100"
      >
        <div class="flex flex-col md:mx-6 md:flex-row">
          <a class="nav-link" href="#">Home</a>
          <a class="nav-link" href="#planos">Planos</a>
          <a class="nav-link" href="#como-funciona">Como funciona</a>
          <a class="nav-link" href="#antes-depois">Resultados</a>
          <a class="nav-link" href="#sobre">Sobre mim</a>
          <a class="nav-link" href="#">Contato</a>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.text-shadow {
  text-shadow:
    0 0 5px #000,
    0 0 10px #000,
    0 0 15px #153e9d,
    0 0 15px #153e9d,
    0 0 20px #153e9d;
}

.nav-link {
  @apply text-shadow my-2 transform font-semibold text-gray-200 transition-colors duration-300 hover:text-blue-400 md:mx-4 md:my-0;
}
</style>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
</script>

<template>
  <nav class="relative bg-gray-800">
    <div class="container px-6 py-4 mx-auto md:flex md:justify-between md:items-center">
      <div class="flex items-center justify-between">
        <a href="#">
          <img class="w-auto h-20" src="/logo.png" alt="" />
        </a>
        <div class="flex lg:hidden">
          <button
            @click="isOpen = !isOpen"
            type="button"
            class="text-gray-200 hover:text-gray-400 focus:outline-none focus:text-gray-400"
            aria-label="toggle menu"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-6 h-6"
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
              class="w-6 h-6"
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
        class="absolute inset-x-0 z-20 w-full bg-gray-800 px-6 py-4 transition-all duration-300 ease-in-out md:mt-0 md:p-0 md:top-0 md:relative md:bg-transparent md:w-auto md:opacity-100 md:translate-x-0 md:flex md:items-center"
      >
        <div class="flex flex-col md:flex-row md:mx-6">
          <a
            class="my-2 transition-colors duration-300 transform text-gray-200 hover:text-blue-400 md:mx-4 md:my-0 font-semibold"
            href="#"
            >Home</a
          >
          <a
            class="my-2 transition-colors duration-300 transform text-gray-200 hover:text-blue-400 md:mx-4 md:my-0 font-semibold"
            href="#"
            >Planos</a
          >
          <a
            class="my-2 transition-colors duration-300 transform text-gray-200 hover:text-blue-400 md:mx-4 md:my-0 font-semibold"
            href="#"
            >Contato</a
          >
          <a
            class="my-2 transition-colors duration-300 transform text-gray-200 hover:text-blue-400 md:mx-4 md:my-0 font-semibold"
            href="#"
            >Sobre</a
          >
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped></style>

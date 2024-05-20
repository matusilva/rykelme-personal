<script setup>
import { RiWhatsappLine } from '@remixicon/vue'
</script>

<template>
  <header
    class="bg-no-repeat bg-center bg-cover"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)),
        url(/background.jpeg);
    "
  >
    <div class="container px-6 mx-auto">
      <div class="items-center lg:flex">
        <div class="w-full lg:w-1/2">
          <div class="lg:max-w-lg">
            <h1 class="text-3xl font-semibold text-white lg:text-4xl pt-4 sm:pt-1 text-shadow">
              CONSULTORIA COMPLETA TREINAMENTO PERSONALIZADO E ACOMPANHAMENTO <br />
              <span class="text-blue-500">ESPECIALIZADO</span>
            </h1>
            <p class="mt-3 text-gray-400">Especialista em</p>

            <div class="mt-4 space-y-5">
              <p class="flex items-center -mx-2 text-gray-700 dark:text-gray-200">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="w-6 h-6 mx-2 text-blue-500"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"
                  />
                </svg>

                <span class="mx-2">emagrecimento e definição muscular</span>
              </p>

              <p class="flex items-center -mx-2 text-gray-700 dark:text-gray-200">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="w-6 h-6 mx-2 text-blue-500"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"
                  />
                </svg>

                <span class="mx-2">hipertrofia muscular</span>
              </p>

              <p class="flex items-center -mx-2 text-gray-700 dark:text-gray-200">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="w-6 h-6 mx-2 text-blue-500"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"
                  />
                </svg>

                <span class="mx-2">posturologia e reabilitação de lesões</span>
              </p>
            </div>

            <button
              class="flex items-center mt-4 px-4 py-2 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-600 rounded-lg hover:bg-blue-500 focus:outline-none focus:ring focus:ring-blue-300 focus:ring-opacity-80"
            >
              <RiWhatsappLine class="w-5 h-5 mx-1" />
              <span class="mx-1">Entrar em contato</span>
            </button>
          </div>
        </div>
        <div class="flex items-center justify-center w-full mt-6 lg:mt-0 lg:w-1/2">
          <img class="w-full h-full lg:max-w-sm" src="/profile.png" alt="profile" />
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.text-shadow {
  text-shadow:
    0 0 5px #000,
    0 0 10px #000,
    0 0 15px #153e9d,
    0 0 20px #153e9d; /* Azul claro */
}
</style>

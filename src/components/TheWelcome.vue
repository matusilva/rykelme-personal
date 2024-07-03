<script setup>
import { ref } from 'vue'
import { RiWhatsappLine } from '@remixicon/vue'

const especialidades = ref([
  'emagrecimento e definição muscular',
  'hipertrofia muscular',
  'posturologia e reabilitação de lesões'
])
</script>

<template>
  <header
    class="bg-cover bg-center bg-no-repeat"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)),
        url(/backgrounds/background.jpeg);
    "
  >
    <div class="container mx-auto px-6">
      <div class="items-center lg:flex">
        <div class="w-full lg:w-1/2">
          <h1
            class="text-shadow animate__animated animate__fadeInRight pt-4 text-3xl font-semibold text-white sm:pt-0 lg:text-5xl"
          >
            CONSULTORIA COMPLETA TREINAMENTO PERSONALIZADO E ACOMPANHAMENTO <br />
            <p class="text-blue-500">ESPECIALIZADO</p>
          </h1>
          <p class="animate__animated animate__fadeInRight animate__slow mt-3 text-gray-400">
            Especialista em
          </p>

          <div class="animate__animated animate__fadeInRight animate__slower mt-4 space-y-5">
            <p
              v-for="especialidade in especialidades"
              :key="especialidade"
              class="-mx-2 flex items-center text-gray-200"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="mx-2 h-6 w-6 text-blue-500"
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
              <span class="mx-2 text-white">{{ especialidade }}</span>
            </p>
          </div>

          <a
            href="https://wa.me/558499149515?text=Ol%C3%A1,+gostaria+de+mais+informa%C3%A7%C3%B5es+sobre+a+consultoria"
            target="_blank"
          >
            <button
              class="animate__animated animate__fadeIn animate__slower mt-4 flex transform items-center rounded-lg bg-blue-600 px-4 py-2 font-medium capitalize tracking-wide text-white transition duration-500 ease-in-out hover:scale-110 hover:bg-blue-500 focus:outline-none focus:ring focus:ring-blue-300 focus:ring-opacity-80"
            >
              <RiWhatsappLine class="mx-1 h-5 w-5" />
              <span class="mx-1">Entrar em contato</span>
            </button>
          </a>
        </div>
        <div
          class="animate__animated animate__fadeInRightBig flex w-full items-center justify-end lg:mt-0 lg:w-1/2"
        >
          <img class="lg:max-w-md" src="/profile/profile.png" alt="profile" />
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
    0 0 15px #153e9d,
    0 0 20px #153e9d;
}
</style>

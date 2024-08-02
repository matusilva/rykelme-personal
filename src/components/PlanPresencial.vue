<script setup>
import { onMounted } from 'vue'
import { gsap } from 'gsap'
import IconCheck from '@/components/icons/IconCheck.vue'

const list = [
  'Anamnese',
  'Avaliação postural',
  'Avaliação física',
  'Treino personalizado',
  'Suporte via WhatsApp',
  'Aplicativo com vídeos explicativos'
]

onMounted(() => {
  gsap.from('.animatePlan .plan-item', {
    scrollTrigger: {
      trigger: '.animatePlan',
      start: 'top 80%',
      end: 'bottom 20%',
      toggleActions: 'play none none reverse'
    },
    opacity: 0,
    y: 250,
    duration: 1,
    stagger: 0.5
  })
})
</script>

<template>
  <section id="planos" class="bg-gray-900">
    <div class="container mx-auto px-6 py-10">
      <h1 class="text-center text-2xl font-semibold text-white lg:text-3xl">
        Consulte os <br />Planos e Valores
      </h1>

      <div class="mt-2 text-center">
        <span class="inline-block h-1 w-40 rounded-full bg-[#0099FF]"></span>
        <span class="ml-1 inline-block h-1 w-3 rounded-full bg-[#0099FF]"></span>
        <span class="ml-1 inline-block h-1 w-1 rounded-full bg-[#0099FF]"></span>
      </div>
    </div>

    <div class="container mx-auto px-6 pb-8">
      <div class="mx-auto max-w-2xl overflow-hidden rounded-lg bg-gray-800 p-1.5">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="flex transform items-center justify-center rounded-lg bg-gray-600 bg-transparent px-3 py-2 font-medium uppercase text-gray-200 transition-colors duration-300 focus:outline-none"
          >
            Pacotes e Planos
          </div>
        </div>
      </div>

      <div
        class="animatePlan mt-4 flex flex-col items-center justify-center space-y-6 lg:-mx-5 lg:flex-row lg:space-y-0"
      >
        <div
          class="plan-item w-full transform rounded-lg bg-gray-50 px-6 py-4 transition-colors duration-500 lg:mx-5 lg:w-96 dark:bg-gray-800"
        >
          <div class="text-center">
            <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Mensal</p>
            <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Presencial</p>
            <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">R$ 500/Mês</h4>
            <p class="mt-4 text-gray-500 dark:text-gray-300">4 semanas de treino</p>
          </div>

          <div class="mt-8 space-y-8">
            <div v-for="(item, key) in list" :key="key" class="flex items-center">
              <IconCheck /> <span class="mx-4 text-gray-700 dark:text-gray-300">{{ item }}</span>
            </div>
          </div>

          <a
            href="https://wa.me/558499149515?text=Olá, eu gostaria de saber mais sobre o Plano Mensal"
            target="_blank"
          >
            <button
              class="mt-10 w-full transform rounded-md bg-blue-500 px-4 py-2 font-medium capitalize tracking-wide text-white transition duration-500 ease-in-out hover:scale-110 hover:bg-blue-600 focus:bg-blue-600 focus:outline-none"
            >
              Escolher Plano Mensal
            </button>
          </a>
        </div>

        <div
          class="plan-item w-full transform rounded-lg bg-gray-50 px-6 py-4 transition-colors duration-500 lg:mx-5 lg:w-96 dark:bg-gray-800"
        >
          <div class="text-center">
            <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Trimestral</p>
            <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Presencial</p>
            <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">R$ 400/Mês</h4>
            <p class="mt-4 text-gray-500 dark:text-gray-300">12 semanas de treino</p>
          </div>

          <div class="mt-8 space-y-8">
            <div v-for="(item, key) in list" :key="key" class="flex items-center">
              <IconCheck /> <span class="mx-4 text-gray-700 dark:text-gray-300">{{ item }}</span>
            </div>
          </div>

          <a
            href="https://wa.me/558499149515?text=Olá, eu gostaria de saber mais sobre o Plano Trimestral"
            target="_blank"
          >
            <button
              class="mt-10 w-full transform rounded-md bg-blue-500 px-4 py-2 font-medium capitalize tracking-wide text-white transition duration-500 ease-in-out hover:scale-110 hover:bg-blue-600 focus:bg-blue-600 focus:outline-none"
            >
              Escolher Plano Trimestral
            </button>
          </a>
        </div>

        <div
          class="plan-item w-full transform overflow-hidden rounded-lg bg-gray-50 transition-colors duration-500 lg:mx-5 lg:w-96 dark:bg-gray-800"
        >
          <div class="px-6 py-4">
            <div class="text-center">
              <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Semestral</p>
              <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Presencial</p>
              <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">
                R$ 350/Mês
              </h4>
              <p class="mt-4 text-gray-500 dark:text-gray-300">24 semanas de treino</p>
            </div>

            <div class="mt-8 space-y-8">
              <div v-for="(item, key) in list" :key="key" class="flex items-center">
                <IconCheck />
                <span class="mx-4 text-gray-700 dark:text-gray-300">{{ item }}</span>
              </div>
            </div>

            <a
              href="https://wa.me/558499149515?text=Olá, eu gostaria de saber mais sobre o Plano Semestral"
              target="_blank"
            >
              <button
                class="mt-10 w-full transform rounded-md bg-blue-500 px-4 py-2 font-medium capitalize tracking-wide text-white transition duration-500 ease-in-out hover:scale-110 hover:bg-blue-600 focus:bg-blue-600 focus:outline-none"
              >
                Escolher Plano Semestral
              </button>
            </a>
          </div>
        </div>

        <div
          class="plan-item w-full transform overflow-hidden rounded-lg bg-gray-50 transition-colors duration-500 lg:mx-5 lg:w-96 dark:bg-gray-800"
        >
          <p class="bg-blue-800 py-1 text-center text-sm uppercase tracking-widest text-white">
            Maior Desconto
          </p>
          <div class="px-6 py-4">
            <div class="text-center">
              <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Anual</p>
              <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Presencial</p>
              <!-- <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">6x R$150,00</h4> -->
              <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">
                R$ 300/Mês
              </h4>
              <p class="mt-4 text-gray-500 dark:text-gray-300">48 semanas de treino</p>
            </div>

            <div class="mt-8 space-y-8">
              <div v-for="(item, key) in list" :key="key" class="flex items-center">
                <IconCheck />
                <span class="mx-4 text-gray-700 dark:text-gray-300">{{ item }}</span>
              </div>
            </div>

            <a
              href="https://wa.me/558499149515?text=Olá, eu gostaria de saber mais sobre o Plano Anual"
              target="_blank"
            >
              <button
                class="mt-10 w-full transform rounded-md bg-blue-500 px-4 py-2 font-medium capitalize tracking-wide text-white transition duration-500 ease-in-out hover:scale-110 hover:bg-blue-600 focus:bg-blue-600 focus:outline-none"
              >
                Escolher Plano Anual
              </button>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

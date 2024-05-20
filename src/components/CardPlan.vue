<script setup>
const props = defineProps(['activeTab'])
</script>

<template>
  <div
    v-if="props.activeTab === 'Prata'"
    class="flex flex-col items-center justify-center mt-16 space-y-6 md:items-start md:-mx-5 md:space-y-0 md:flex-row"
  >
    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Mensal</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">1x R$200,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">1x R$200,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">6 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Mensal
      </button>
    </div>

    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Trimestral</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">3x R$137,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">3x R$137,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">12 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Trimestral
      </button>
    </div>

    <div
      class="w-full overflow-hidden transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <p class="py-2 text-sm text-center text-white uppercase bg-blue-500">Mais Recomendado</p>
      <div class="px-6 py-4">
        <div class="text-center">
          <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Semestral</p>
          <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
          <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">6x R$97,00</h4>
          <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">6x R$97,00</h4>
          <p class="mt-4 text-gray-500 dark:text-gray-300">24 semanas de treino</p>
        </div>

        <div class="mt-8 space-y-8">
          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300"
              >Aplicativo com vídeos explicativos</span
            >
          </div>
        </div>

        <button
          class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
        >
          Escolher Plano Semestral
        </button>
      </div>
    </div>
  </div>

  <div
    v-if="props.activeTab === 'Ouro'"
    class="flex flex-col items-center justify-center mt-16 space-y-6 md:items-start md:-mx-5 md:space-y-0 md:flex-row"
  >
    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Mensal</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">1x R$300,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">1x R$300,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">6 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Direito a 1 vídeo chamada para tirar dúvidas</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Mensal
      </button>
    </div>

    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Trimestral</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">3x R$237,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">3x R$237,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">12 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Direito a 2 vídeo chamada para tirar dúvidas</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Trimestral
      </button>
    </div>

    <div
      class="w-full overflow-hidden transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <p class="py-2 text-sm text-center text-white bg-blue-500">BÔNUS: Receba um Ebook.</p>
      <div class="px-6 py-4">
        <div class="text-center">
          <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Semestral</p>
          <p class="mt-4 text-gray-500 dark:text-gray-300">Consultoria Online</p>
          <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">6x R$197,00</h4>
          <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">6x R$197,00</h4>
          <p class="mt-4 text-gray-500 dark:text-gray-300">24 semanas de treino</p>
        </div>

        <div class="mt-8 space-y-8">
          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300"
              >Aplicativo com vídeos explicativos</span
            >
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300"
              >Direito a 4 vídeo chamada para tirar dúvidas</span
            >
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300"
              >Bônus: Ebook "Dominando a técnica dos exercícios da musculação".</span
            >
          </div>
        </div>

        <button
          class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
        >
          Escolher Plano Semestral
        </button>
      </div>
    </div>
  </div>

  <div
    v-if="props.activeTab === 'Diamante'"
    class="flex flex-col items-center justify-center mt-16 space-y-6 md:items-start md:-mx-5 md:space-y-0 md:flex-row"
  >
    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Mensal</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Acompanhamento Presencial</p>
        <p class="text-gray-500 dark:text-gray-300">3x na semana</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">1x R$400,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">1x R$400,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">6 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação física</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Mensal
      </button>
    </div>

    <div
      class="w-full px-6 py-4 transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="text-center">
        <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Trimestral</p>
        <p class="mt-4 text-gray-500 dark:text-gray-300">Acompanhamento Presencial</p>
        <p class="text-gray-500 dark:text-gray-300">3x na semana</p>
        <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">3x R$337,00</h4>
        <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">3x R$337,00</h4>
        <p class="mt-4 text-gray-500 dark:text-gray-300">18 semanas de treino</p>
      </div>

      <div class="mt-8 space-y-8">
        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação física</span>
        </div>

        <div class="flex items-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-blue-500"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
              clip-rule="evenodd"
            />
          </svg>

          <span class="mx-4 text-gray-700 dark:text-gray-300"
            >Aplicativo com vídeos explicativos</span
          >
        </div>
      </div>

      <button
        class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
      >
        Escolher Plano Trimestral
      </button>
    </div>

    <div
      class="w-full overflow-hidden transition-colors duration-300 transform rounded-lg md:mx-5 md:w-96 bg-gray-50 dark:bg-gray-800"
    >
      <div class="px-6 py-4">
        <div class="text-center">
          <p class="text-2xl font-semibold text-gray-800 dark:text-gray-100">Plano Semestral</p>
          <p class="mt-4 text-gray-500 dark:text-gray-300">Acompanhamento Presencial</p>
          <p class="text-gray-500 dark:text-gray-300">3x na semana</p>
          <h4 class="mt-2 text-gray-600 line-through dark:text-gray-400">6x R$300,00</h4>
          <h4 class="mt-2 text-4xl font-semibold text-gray-800 dark:text-gray-100">6x R$300,00</h4>
          <p class="mt-4 text-gray-500 dark:text-gray-300">24 semanas de treino</p>
        </div>

        <div class="mt-8 space-y-8">
          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Anamnese</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Treino personalizado</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Suporte via WhatsApp</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação postural</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300">Avaliação física</span>
          </div>

          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5 text-blue-500"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                clip-rule="evenodd"
              />
            </svg>

            <span class="mx-4 text-gray-700 dark:text-gray-300"
              >Aplicativo com vídeos explicativos</span
            >
          </div>
        </div>

        <button
          class="w-full px-4 py-2 mt-10 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-500 rounded-md hover:bg-blue-600 focus:outline-none focus:bg-blue-600"
        >
          Escolher Plano Semestral
        </button>
      </div>
    </div>
  </div>
</template>

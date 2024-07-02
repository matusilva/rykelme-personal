<script setup>
import CardPlan from '@/components/CardPlan.vue'
import { RiAwardFill, RiMedalLine, RiVipDiamondLine } from '@remixicon/vue'
</script>

<template>
  <section id="planos" class="bg-gray-900">
    <div class="container px-6 py-10 mx-auto">
      <h1 class="text-center text-2xl font-semibold lg:text-3xl text-white">
        Consulte os <br />Planos e Valores
      </h1>

      <div class="text-center mt-2">
        <span class="inline-block w-40 h-1 bg-blue-500 rounded-full"></span>
        <span class="inline-block w-3 h-1 ml-1 bg-blue-500 rounded-full"></span>
        <span class="inline-block w-1 h-1 ml-1 bg-blue-500 rounded-full"></span>
      </div>
    </div>

    <div class="container px-6 pb-8 mx-auto">
      <div class="max-w-2xl p-1.5 mx-auto overflow-hidden rounded-lg bg-gray-800">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="flex items-center justify-center px-3 py-2 font-medium uppercase transition-colors duration-300 transform bg-transparent rounded-lg focus:outline-none text-gray-200 bg-gray-600"
          >
            Consultoria Prata
            <RiAwardFill class="ml-1" />
          </div>
        </div>
      </div>
      <CardPlan activeTab="Prata" />
    </div>

    <div class="container px-6 pb-8 mx-auto">
      <div class="max-w-2xl p-1.5 mx-auto overflow-hidden rounded-lg bg-gray-800">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="text-yellow-400 bg-gray-700 flex items-center justify-center px-3 py-2 font-medium uppercase transition-colors duration-300 transform bg-transparent rounded-lg focus:outline-none"
          >
            Consultoria Ouro
            <RiMedalLine class="ml-1" />
          </div>
        </div>
      </div>
      <CardPlan activeTab="Ouro" />
    </div>

    <div class="container px-6 pb-8 mx-auto">
      <div class="max-w-2xl p-1.5 mx-auto overflow-hidden rounded-lg bg-gray-800">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="text-cyan-300 flex items-center justify-center px-3 py-2 font-medium uppercase transition-colors duration-300 transform bg-transparent rounded-lg focus:outline-none bg-gray-700"
          >
            Consultoria Diamante
            <RiVipDiamondLine class="ml-1" />
          </div>
        </div>
      </div>
      <CardPlan activeTab="Diamante" />
    </div>
  </section>
</template>

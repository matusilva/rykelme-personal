<script setup>
import CardPlan from '@/components/CardPlan.vue'
import { RiAwardFill, RiMedalLine, RiVipDiamondLine } from '@remixicon/vue'
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
            Consultoria Prata
            <RiAwardFill class="ml-1" />
          </div>
        </div>
      </div>
      <CardPlan activeTab="Prata" />
    </div>

    <div class="container mx-auto px-6 pb-8">
      <div class="mx-auto max-w-2xl overflow-hidden rounded-lg bg-gray-800 p-1.5">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="flex transform items-center justify-center rounded-lg bg-gray-700 bg-transparent px-3 py-2 font-medium uppercase text-yellow-400 transition-colors duration-300 focus:outline-none"
          >
            Consultoria Ouro
            <RiMedalLine class="ml-1" />
          </div>
        </div>
      </div>
      <CardPlan activeTab="Ouro" />
    </div>

    <div class="container mx-auto px-6 pb-8">
      <div class="mx-auto max-w-2xl overflow-hidden rounded-lg bg-gray-800 p-1.5">
        <div class="grid gap-3 sm:grid-cols-1">
          <div
            class="flex transform items-center justify-center rounded-lg bg-gray-700 bg-transparent px-3 py-2 font-medium uppercase text-cyan-300 transition-colors duration-300 focus:outline-none"
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

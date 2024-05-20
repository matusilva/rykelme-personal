<script setup>
import { ref } from 'vue'
import CardPlan from '@/components/CardPlan.vue'
import { RiAwardFill, RiMedalLine, RiVipDiamondLine } from '@remixicon/vue'

const tabs = ['Prata', 'Ouro', 'Diamante']
const activeTab = ref(tabs[1])
</script>

<template>
  <section class="bg-gray-900">
    <div class="container px-6 py-8 mx-auto">
      <div class="max-w-2xl p-1.5 mx-auto overflow-hidden rounded-lg bg-gray-800">
        <div class="grid gap-3 md:grid-cols-3">
          <button
            v-for="(tab, key) in tabs"
            :key="key"
            @click="activeTab = tab"
            class="flex items-center justify-center px-3 py-2 font-medium uppercase transition-colors duration-300 transform bg-transparent rounded-lg focus:outline-none text-gray-200 hover:bg-gray-600"
            :class="{ 'bg-gray-500': activeTab === tab }"
          >
            {{ tab }}
            <RiAwardFill v-if="tab === 'Prata'" class="ml-1" />
            <RiMedalLine v-if="tab === 'Ouro'" class="ml-1" />
            <RiVipDiamondLine v-if="tab === 'Diamante'" class="ml-1" />
          </button>
        </div>
      </div>
      <CardPlan :active-tab="activeTab" />
    </div>
  </section>
</template>

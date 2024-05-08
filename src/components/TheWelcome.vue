<script setup>
import { RiInstagramLine, RiWhatsappLine } from '@remixicon/vue'
</script>

<template>
  <header class="bg-gray-900">
    <div class="container px-6 mx-auto">
      <div class="items-center lg:flex">
        <div class="w-full lg:w-1/2">
          <div class="lg:max-w-lg">
            <h1 class="text-3xl font-semibold text-white lg:text-4xl">
              Lorem ipsum dolor <br />
              your <span class="text-blue-500">Personal</span>
            </h1>
            <p class="mt-3 text-gray-400">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro beatae error laborum
              ab amet sunt recusandae? Reiciendis natus perspiciatis optio.
            </p>
            <button
              class="flex items-center px-4 py-2 mt-6 font-medium tracking-wide text-white capitalize transition-colors duration-300 transform bg-blue-600 rounded-lg hover:bg-blue-500 focus:outline-none focus:ring focus:ring-blue-300 focus:ring-opacity-80"
            >
              <RiWhatsappLine /> <span class="mx-1">Contato</span>
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

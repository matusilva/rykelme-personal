<script setup>
import { RiInstagramLine, RiGithubFill, RiWhatsappLine } from '@remixicon/vue'
</script>
<template>
  <footer class="bg-gray-800">
    <div
      class="container mx-auto flex flex-col items-center justify-between space-y-4 p-6 sm:flex-row sm:space-y-0"
    >
      <p class="text-sm text-gray-300">© Copyright 2021. Todos os direitos reservados.</p>

      <div class="-mx-2 flex">
        <a
          href="https://www.instagram.com/rykelmelucas_/"
          target="_blank"
          class="mx-2 text-gray-300 transition-colors duration-300 hover:text-blue-400"
          aria-label="Instagram"
        >
          <RiInstagramLine />
        </a>
        <a
          href="https://wa.me/558499149515"
          target="_blank"
          class="mx-2 text-gray-300 transition-colors duration-300 hover:text-blue-400"
          aria-label="WhatsApp"
        >
          <RiWhatsappLine />
        </a>
      </div>

      <p class="flex items-center text-xs text-gray-300">
        Desenvolvido:
        <a
          href="https://github.com/matusilva"
          target="_blank"
          class="mx-2 flex text-gray-300 transition-colors duration-300 hover:text-blue-400"
          aria-label="Github"
        >
          <RiGithubFill /> <span class="mx-1 flex items-center">Matheus Silva</span>
        </a>
      </p>
    </div>
  </footer>
</template>

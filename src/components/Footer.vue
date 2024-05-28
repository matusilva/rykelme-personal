<script setup>
import { RiInstagramLine, RiGithubFill, RiWhatsappLine } from '@remixicon/vue'
</script>
<template>
  <footer class="bg-gray-800">
    <div
      class="container flex flex-col items-center justify-between p-6 mx-auto space-y-4 sm:space-y-0 sm:flex-row"
    >
      <p class="text-sm text-gray-300">© Copyright 2021. Todos os direitos reservados.</p>

      <div class="flex -mx-2">
        <a
          href="https://www.instagram.com/rykelmelucas_/"
          target="_blank"
          class="mx-2 transition-colors duration-300 text-gray-300 hover:text-blue-400"
          aria-label="Instagram"
        >
          <RiInstagramLine />
        </a>
        <a
          href="https://wa.me/558499149515"
          target="_blank"
          class="mx-2 transition-colors duration-300 text-gray-300 hover:text-blue-400"
          aria-label="WhatsApp"
        >
          <RiWhatsappLine />
        </a>
      </div>

      <p class="text-xs text-gray-300 flex items-center">
        Desenvolvido:
        <a
          href="https://github.com/matusilva"
          target="_blank"
          class="mx-2 transition-colors duration-300 text-gray-300 hover:text-blue-400 flex"
          aria-label="Github"
        >
          <RiGithubFill /> <span class="mx-1 flex items-center">Matheus Silva</span>
        </a>
      </p>
    </div>
  </footer>
</template>

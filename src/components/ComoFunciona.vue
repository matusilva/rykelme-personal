<script setup>
import { RiCheckLine } from '@remixicon/vue'
</script>

<template>
  <section
    id="como-funciona"
    class="bg-no-repeat bg-cover bg-right-top"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.8)),
        url(/background-woman.jpg);
    "
  >
    <div class="container flex flex-col px-6 mx-auto space-y-6 h-full py-16 lg:h-[32rem]">
      <div class="w-full">
        <h1
          class="text-3xl font-semibold tracking-wide text-white lg:text-4xl text-center text-shadow"
        >
          COMO FUNCIONA A CONSULTORIA
        </h1>
        <div class="grid gap-6 mt-8 sm:grid-cols-2">
          <div class="flex items-center text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Anamnese completa para entender suas necessidades e histórico de saúde.</span
            >
          </div>

          <div class="flex items-center -px-3 text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Avaliação Física e Postural com diagnóstico preciso para identificar suas
              necessidades específicas.</span
            >
          </div>

          <div class="flex items-center -px-3 text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Treino personalizado, adaptado aos seus objetivos e necessidades individuais.</span
            >
          </div>

          <div class="flex items-center -px-3 text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Aplicativo com vídeos explicativos dos exercícios, garantindo a execução
              correta.</span
            >
          </div>

          <div class="flex items-center -px-3 text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Suporte via <span class="green-whatsapp">WhatsApp</span> 24 horas por dia para tirar
              dúvidas e oferecer apoio constante.</span
            >
          </div>

          <div class="flex items-center -px-3 text-gray-200">
            <RiCheckLine />
            <span class="mx-3"
              >Ebook "Dominando a Técnica dos Exercícios de Musculação", com dicas para evitar
              lesões e manter uma boa postura durante os treinos.</span
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.text-shadow {
  text-shadow:
    0 0 10px #000,
    0 0 20px #000,
    0 0 30px #00aaff,
    0 0 40px #00aaff,
    0 0 70px #00aaff,
    0 0 80px #000,
    0 0 100px #000,
    0 0 150px #fff;
}
.green-whatsapp {
  color: #27d367;
}
</style>

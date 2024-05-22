<script setup>
import { RiCheckLine } from '@remixicon/vue'

const items = [
  'Anamnese completa para entender suas necessidades e histórico de saúde.',
  'Avaliação Física e Postural com diagnóstico preciso para identificar suas necessidades específicas.',
  'Treino personalizado, adaptado aos seus objetivos e necessidades individuais.',
  'Aplicativo com vídeos explicativos dos exercícios, garantindo a execução correta.',
  'Suporte via WhatsApp 24 horas por dia para tirar dúvidas e oferecer apoio constante.',
  "Ebook 'Dominando a Técnica dos Exercícios de Musculação', com dicas para evitar lesões e manter uma boa postura durante os treinos."
]
</script>

<template>
  <section
    id="como-funciona"
    class="bg-no-repeat bg-cover bg-right-top"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url(/backgrounds/background-woman.jpg);
    "
  >
    <div class="container flex flex-col px-6 mx-auto space-y-6 h-full py-16 lg:h-[48rem]">
      <div class="w-full">
        <h1
          class="text-3xl font-semibold tracking-wide text-white py-4 lg:text-5xl text-center text-shadow"
        >
          COMO FUNCIONA A CONSULTORIA
        </h1>
        <div class="grid gap-6 mt-8 md:text-xl">
          <template v-for="(item, key) in items" :key="key">
            <div class="flex items-center">
              <RiCheckLine size="32" class="text-blue-500" />
              <span class="mx-3 text-gray-200">{{ item }}</span>
            </div>
          </template>
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

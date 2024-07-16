<script setup>
import { onMounted } from 'vue'
import { gsap } from 'gsap'
import { RiCheckLine } from '@remixicon/vue'

const items = [
  'Anamnese completa para entender suas necessidades e histórico de saúde.',
  'Avaliação Física e Postural com diagnóstico preciso para identificar suas necessidades específicas.',
  'Treino personalizado, adaptado aos seus objetivos e necessidades individuais.',
  'Aplicativo com vídeos explicativos dos exercícios, garantindo a execução correta.',
  'Suporte via WhatsApp 24 horas por dia para tirar dúvidas e oferecer apoio constante.',
  "Ebook 'Dominando a Técnica dos Exercícios de Musculação', com dicas para evitar lesões e manter uma boa postura durante os treinos."
]

onMounted(() => {
  gsap.utils.toArray('.item').forEach((item) => {
    gsap.from(item, {
      scrollTrigger: {
        trigger: item,
        start: 'top 80%',
        end: 'top 20%',
        toggleActions: 'play none none reverse'
      },
      opacity: 0,
      x: -200,
      duration: 1,
      stagger: 0.3
    })
  })
})
</script>

<template>
  <section
    id="como-funciona"
    class="relative bg-cover bg-right-top bg-no-repeat"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url(/backgrounds/background-woman.jpg);
    "
  >
    <div class="container mx-auto flex h-full flex-col space-y-6 px-6 py-16 lg:h-[48rem]">
      <div>
        <h1 class="py-4 text-center text-3xl font-semibold tracking-wide text-white lg:text-5xl">
          COMO FUNCIONA A CONSULTORIA
        </h1>
        <div class="mt-8 grid gap-6 md:text-xl">
          <template v-for="(item, key) in items" :key="key">
            <div class="item flex items-center">
              <RiCheckLine size="32" class="text-[#0099FF]" />
              <span class="mx-3 text-gray-200">{{ item }}</span>
            </div>
          </template>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>

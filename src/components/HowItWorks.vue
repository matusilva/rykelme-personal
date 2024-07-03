<script setup>
import { RiCheckLine } from '@remixicon/vue'
import { ref, onMounted } from 'vue'

const items = [
  'Anamnese completa para entender suas necessidades e histórico de saúde.',
  'Avaliação Física e Postural com diagnóstico preciso para identificar suas necessidades específicas.',
  'Treino personalizado, adaptado aos seus objetivos e necessidades individuais.',
  'Aplicativo com vídeos explicativos dos exercícios, garantindo a execução correta.',
  'Suporte via WhatsApp 24 horas por dia para tirar dúvidas e oferecer apoio constante.',
  "Ebook 'Dominando a Técnica dos Exercícios de Musculação', com dicas para evitar lesões e manter uma boa postura durante os treinos."
]

const isVisible = ref(false)
const sectionRef = ref(null)

// Função para verificar a interseção com o viewport
const checkIntersect = (entries, observer) => {
  entries.forEach((entry) => {
    if (entry.isIntersecting) {
      isVisible.value = true
      observer.unobserve(entry.target)
    }
  })
}

onMounted(() => {
  const options = {
    root: null,
    rootMargin: '-200px 0px',
    threshold: 0.5
  }

  const observer = new IntersectionObserver(checkIntersect, options)
  observer.observe(sectionRef.value)
})
</script>

<template>
  <section
    ref="sectionRef"
    id="como-funciona"
    class="bg-cover bg-right-top bg-no-repeat"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url(/backgrounds/background-woman.jpg);
    "
  >
    <div
      v-if="!isVisible"
      class="bg-cover bg-right-top bg-no-repeat md:p-44"
      style="
        background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
          url(/backgrounds/background-woman.jpg);
      "
    ></div>
    <div
      v-if="isVisible"
      class="animate__animated animate__fadeInRightBig animate__slow container mx-auto flex h-full flex-col space-y-6 px-6 py-16 lg:h-[48rem]"
    >
      <h1
        class="text-shadow py-4 text-center text-3xl font-semibold tracking-wide text-white lg:text-5xl"
      >
        COMO FUNCIONA A CONSULTORIA
      </h1>
      <div class="mt-8 grid gap-6 md:text-xl">
        <template v-for="(item, key) in items" :key="key">
          <div class="flex items-center">
            <RiCheckLine size="32" class="text-blue-500" />
            <span class="mx-3 text-gray-200">{{ item }}</span>
          </div>
        </template>
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

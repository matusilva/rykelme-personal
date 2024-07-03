<script setup>
import { RiCheckLine } from '@remixicon/vue'
import { ref, onMounted, onBeforeUnmount } from 'vue'

const items = [
  'Anamnese completa para entender suas necessidades e histórico de saúde.',
  'Avaliação Física e Postural com diagnóstico preciso para identificar suas necessidades específicas.',
  'Treino personalizado, adaptado aos seus objetivos e necessidades individuais.',
  'Aplicativo com vídeos explicativos dos exercícios, garantindo a execução correta.',
  'Suporte via WhatsApp 24 horas por dia para tirar dúvidas e oferecer apoio constante.',
  "Ebook 'Dominando a Técnica dos Exercícios de Musculação', com dicas para evitar lesões e manter uma boa postura durante os treinos."
]

const isVisible = ref(false)
const containerRef = ref(null)

const handleScroll = () => {
  if (!containerRef.value) return

  const sectionTop = containerRef.value.getBoundingClientRect().top
  const screenHeight = window.innerHeight

  // Quando o topo da seção estiver visível na tela
  if (sectionTop < screenHeight) {
    isVisible.value = true
    window.removeEventListener('scroll', handleScroll) // Remove o listener após a animação aparecer
  }
}

onBeforeUnmount(() => {
  window.removeEventListener('scroll', handleScroll)
})

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
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
    <div
      ref="containerRef"
      class="container mx-auto flex h-full flex-col space-y-6 px-6 py-16 lg:h-[48rem]"
      :class="{ 'animate__animated animate__fadeInRightBig animate__slow': isVisible }"
    >
      <div v-if="isVisible">
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
</style>

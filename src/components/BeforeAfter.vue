<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'

const images = ref([
  { src: '/beforeafter/beforeafter1.jpg', alt: '' },
  { src: '/beforeafter/beforeafter2.jpg', alt: '' },
  { src: '/beforeafter/beforeafter3.jpg', alt: '' },
  { src: '/beforeafter/beforeafter4.jpg', alt: '' },
  { src: '/beforeafter/beforeafter5.jpg', alt: '' },
  { src: '/beforeafter/beforeafter6.jpg', alt: '' },
  { src: '/beforeafter/beforeafter7.jpg', alt: '' },
  { src: '/beforeafter/beforeafter8.jpg', alt: '' },
  { src: '/beforeafter/beforeafter9.jpg', alt: '' },
  { src: '/beforeafter/beforeafter10.jpg', alt: '' },
  { src: '/beforeafter/beforeafter11.jpg', alt: '' },
  { src: '/beforeafter/beforeafter12.jpg', alt: '' }
])

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
    id="antes-depois"
    class="bg-cover"
    style="
      background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url(/beforeafter/background.jpg);
    "
  >
    <div
      ref="containerRef"
      class="container mx-auto px-6 py-10"
      :class="{ 'animate__animated animate__fadeInUp animate__slow': isVisible }"
    >
      <div v-if="isVisible">
        <h1 class="text-shadow text-center text-3xl font-semibold uppercase text-white lg:text-4xl">
          Antes e Depois
        </h1>
        <p class="mx-auto my-6 max-w-2xl text-center text-gray-500 dark:text-gray-300">
          Confira algumas transformações alcançadas pelos alunos que embarcaram na jornada de
          fitness com a minha consultoria. Minha missão é impulsionar cada indivíduo rumo aos seus
          objetivos de saúde e condicionamento físico, e estou orgulhoso de compartilhar alguns dos
          incríveis resultados obtidos
        </p>

        <div class="mt-8 grid grid-cols-1 gap-8 md:mt-16 md:grid-cols-4">
          <div v-for="(image, index) in images" :key="index" class="lg:flex">
            <img
              class="w-full rounded-lg object-cover transition duration-300 ease-in-out hover:scale-125 lg:w-64"
              :src="image.src"
              :alt="image.alt"
            />
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
</style>

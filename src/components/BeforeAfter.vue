<script setup>
import { ref } from 'vue'

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

const showZoom = ref(false)
const zoomedImage = ref({ src: '', alt: '' })

const zoomImage = (index) => {
  showZoom.value = true
  zoomedImage.value = images.value[index]
}

const closeZoom = () => {
  showZoom.value = false
}
</script>

<template>
  <section id="antes-depois" class="bg-white">
    <div class="container px-6 py-10 mx-auto">
      <h1 class="text-3xl lg:text-4xl font-semibold text-blue-500 uppercase text-center">
        Antes e Depois
      </h1>

      <div class="grid grid-cols-1 gap-8 mt-8 md:mt-16 md:grid-cols-4">
        <div v-for="(image, index) in images" :key="index" class="lg:flex">
          <img
            class="object-cover w-full rounded-lg lg:w-64 cursor-pointer"
            :src="image.src"
            :alt="image.alt"
            @click="zoomImage(index)"
          />
        </div>
      </div>

      <transition name="fade">
        <div v-if="showZoom" class="zoom-overlay" @click="closeZoom">
          <img :src="zoomedImage.src" :alt="zoomedImage.alt" class="zoomed-image" />
        </div>
      </transition>
    </div>
  </section>
</template>

<style scoped>
.zoom-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
}

.zoomed-image {
  max-width: 80%;
  max-height: 80%;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter,
.fade-leave-to {
  opacity: 0;
}
</style>

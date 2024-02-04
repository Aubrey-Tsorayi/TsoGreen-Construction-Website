<template>
  <div class="flex-wrap lg:columns-2 lg:mr-10 space-y-5">
    <div class="flex-row">
      <div class="flex justify-center pt-10 lg:pt-36 animate-pulse">
        <h1 class="text-6xl lg:text-8xl font-bold font-title">TSO</h1>
        <h1 class="text-6xl lg:text-8xl font-bold text-green-500 font-title">GREEN</h1>
      </div>
      <div class="flex justify-center pt-2">
        <h1 class="lg:text-2xl italic font-title">"Where Quality is our Speciality"</h1>
      </div>
    </div>
    <div class="p-5 lg:p-0 lg:mr-5">
      <Carousel :autoplay="2000" :wrap-around="true">
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/building1.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</1div> -->
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/building2.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</div> -->
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/building3.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</div> -->
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/building4.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</div> -->
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/pavement.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</div> -->
        </Slide>
        <Slide v-for="slide in 1" :key="slide">
          <img src="../assets/gate.jpg" alt="">
          <!-- <div class="carousel__item">{{ slide }}</div> -->
        </Slide>
        <template #addons>
          <Pagination/>
        </template>
      </Carousel>
    </div>
  </div>
</template>

<script>
import {defineComponent} from 'vue'
import {Carousel, Pagination, Slide} from 'vue3-carousel'

import 'vue3-carousel/dist/carousel.css'

export default defineComponent({
  name: 'Autoplay',
  components: {
    Carousel,
    Slide,
    Pagination,
  },
})
</script>
  
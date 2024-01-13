<template>
    <div class="columns-2 mr-10">
        <div class="flex-row">
            <div class="flex justify-center pt-36 animate-pulse">
                <h1 class="text-7xl font-bold font-title">TSO</h1>
                <h1 class="text-7xl font-bold text-green-500 font-title">GREEN</h1>
            </div>
            <div class="flex justify-center pt-2">
                <h1 class="text-xl italic font-title">"Where Quality is our Speciality"</h1>
            </div>
            <div class="flex justify-center gap-5 pt-8">
                <button class="bg-green-500 p-2 rounded-md font-title text-white">Services</button>
                <button class="bg-green-500 p-2 rounded-md font-title text-white">Get a Qoute</button>
            </div>
        </div>
        <div class="mr-5">
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


                <template #addons>
                    <Pagination />
                </template>
            </Carousel>
        </div>
    </div>
</template>
  
<script>
import { defineComponent } from 'vue'
import { Carousel, Pagination, Slide } from 'vue3-carousel'

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
  
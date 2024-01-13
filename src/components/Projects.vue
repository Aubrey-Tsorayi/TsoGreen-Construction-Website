<script setup>
import Tile from './items/Tile.vue'
const projects = [
    {
        title: "Pick n' Pay",
       img: "building4.jpg"
    },
    {
        title: "Spar",
        img: "building4.jpg"
    }
]
</script>

<template>
    <div class="flex-row pt-5">
        <div class="flex justify-center">
            <transition name="fade-left" appear>
                <h1 class="text-green-500 text-6xl font-bold font-title">Projects</h1>
            </transition>
            
        </div>
        <div class="flex justify-center pt-10 gap-10" >
            <Tile v-for="project in projects" :key="project.title" :title="project.title" :img="project.img"></Tile>
        </div>
    </div>
</template>

<style>
.fade-left-enter-from, .fade-left-leave-to {
    opacity: 0;
    transform: translateX(-100%);
}
.fade-left-enter-to, .fade-left-leave-from {
    opacity: 1;
    transform: translateX(0);
}
.fade-left-enter-active, .fade-left-leave-active {
    transition: opacity 2s, transform 2s;
}
</style>
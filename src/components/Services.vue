<script setup>
import Collection from './items/Collection.vue';
const services = [
    {
        title: "Residential Contracting",
       img: "res.jpg"
    },
    {
        title: "Renovations",
        img: "reno.jpg"
    },
    {
        title: "Building Extensions",
        img: "extenn2.jpg"
    },
    {
        title: "Project Management",
        img: "proj.jpg"
    },
    {
        title: "Sub-contracting",
        img: "sub.jpg"
    },
]

</script>

<template>
    <div class="flex-row p-10">
            <div class="flex justify-center">
                <h1 class="text-green-500 text-4xl font-bold font-title">Our Services</h1>
            </div>
            <div name="columns-2" class="grid grid-cols-2 gap-2 p-5">
                <Collection v-for="service in services" :key="service.title" :title="service.title" :img="service.img"/>
            </div>
    </div>
</template>

<style lang="scss" scoped>

</style>
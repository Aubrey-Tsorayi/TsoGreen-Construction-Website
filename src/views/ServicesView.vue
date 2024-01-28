<script setup>
import Service from '@/components/items/Service.vue';
const services = [
    {
        title: "Residential Contracting",
       img: "res.jpg",
       desc: "Our team possesses a clear understanding of the building processes in creating quality homes for our clients. We are passionate about creating a rewarding construction experience for our clients, vendors and stakeholders."
    },
    {
        title: "Renovations",
        img: "reno.jpg",
        desc:"We transform home and office spaces by combining our client's vision with our expertise in creating beautiful and functional spaces."
    },
    {
        title: "Office Space & Building Extensions",
        img: "extenn2.jpg",
        desc: "No matter the function or purpose of the space required, TSOGREEN is determined to seamlessly blend the old with the new structures. Alternatively, we also bring new life into old buildings by enhancing functionality and comfort for modern living."
    },
    {
        title: "Project Management",
        img: "proj.jpg",
        desc: "Where you are building cluster homes, commercial structures, school, warehouses, etc, TSOGREEN's Project Management department is available to add value from the planning stage to execution of larger projects. Our team is dedicated to meet the completion date of each project the team embarks on."
    },
    {
        title: "Sub-contracting",
        img: "sub.jpg",
        desc: "Where a project may require qualified tradesmen, TSOGREEN takes on jobs as a sub-contractor for the following trades: brickwork, concrete works, steel fixing, flooring, plastering, skimming, tiling, painting, ceilings, roofing, carpentry and paving."
    },
]
</script>

<template>
    <div class="flex-row pt-5">
        <div class="flex justify-center py-2">
            <h1 class="font-title font-bold text-4xl text-green-500">Our Services</h1>
        </div>
        <hr class="w-52 lg:w-80 h-1 mx-auto my-3 border-0 rounded md:my-10 bg-gray-700">
        <div class="py-5">
            <Service v-for="service in services" :key="service.title" :title="service.title" :img="service.img" :desc="service.desc"/>
        </div>
        <div class="flex justify-center py-5">
            <button class="bg-green-500 p-3 rounded text-white font-title hover:scale-110">Get a Qoute</button>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>
<script setup>
//define props
const props = defineProps({
    title: String,
    img: String
})

function getImgURl() {
    return new URL(`../../assets/${props.img}`, import.meta.url)
}

</script>

<template>
    <div class="relative group transition ease-in-out delay-75 hover:-translate-y-1 hover:scale-110 duration-300">
        <img :src="getImgURl()" height="80" class="w-60 h-72 rounded-md hover:opacity-45" alt="project">
        <h1 class="invisible absolute text-2xl top-1/2 left-1/4 group-hover:visible font-tile" >{{ title }}</h1>
    </div>
</template>


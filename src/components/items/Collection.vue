<script setup>
const props = defineProps({
    title: String,
    img: String,
})

function getImgURl() {
    return new URL(`../../assets/${props.img}`, import.meta.url)
}

</script>

<template>
    <div class="flex-wrap lg:flex group scale-75 lg:ml-20 pt-10 hover:scale-90 bg-gray-100 rounded-2xl shadow-xl">
        <div class="flex-row lg:flex items-center gap-5 p-5">
            <div>
                <img :src="getImgURl()" class="w-60 rounded-lg shadow-lg " alt="">
            </div>
            <div class="items-center">
                <h1 class="text-3xl font-bold text-center lg:text-left font-title group-hover:text-green-500 ">{{ title }}</h1>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>
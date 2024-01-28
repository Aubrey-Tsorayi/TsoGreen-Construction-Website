<script setup>
const props = defineProps({
    title: String,
    img: String,
    desc: String,
})

function getImgURl() {
    return new URL(`../../assets/${props.img}`, import.meta.url)
}

</script>

<template>
    <div class="flex group scale-90 lg:ml-20 py-2 lg:py10">
        <div class="flex-row space-y-5 lg:flex text-center lg:text-left items-center gap-5 p-5">
            <div class="flex justify-center">
                <img :src="getImgURl()" class="w-60 rounded-lg shadow-lg " alt="">
            </div>
            <div class="flex-row">
                <div class="lg:flex">
                    <h1 class="text-3xl font-bold font-title group-hover:text-green-500 ">{{ title }}</h1>
                </div>
                <div>
                    <p class="text-lg font-title">{{ desc }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>
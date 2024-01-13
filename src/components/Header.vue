<script setup>
import { Icon } from '@iconify/vue';
</script>


<template>
    <header class="flex justify-between bg-green-500 p-2 text-white"> 
        <div class="ml-20">
            <ul class="flex space-x-4 font-title">
                <li>+263 77 210 4560</li>
                <li>johndoe@example.com</li>
                <li>Harare, Zimbabwe</li>
            </ul>
        </div>
        <div class="mr-20">
            <ul class="flex space-x-4">
                <li><Icon icon="teenyicons:facebook-solid" width="22" /></li>
                <li><Icon icon="teenyicons:instagram-solid" width="22" /></li>
                <li><Icon icon="teenyicons:twitter-solid" width="22" /></li>
            </ul>
        </div>
    </header>
</template>


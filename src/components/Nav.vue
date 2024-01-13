<script setup>

</script>

<template>
    <nav class="flex justify-between p-1">
        <div class="ml-20 items-center">
            <img src="../assets/logo.jpg" alt="" width="80" >
        </div>
        <div class="flex items-center space-x-6 mr-20">
            <ul class="flex space-x-8 text-lg">
                <RouterLink to="/" class="hover:text-green-500 hover:cursor-pointer font-title">Home</RouterLink>
                <RouterLink to="/about" class="hover:text-green-500 hover:cursor-pointer font-title">About Us</RouterLink>
                <RouterLink to="/services" class="hover:text-green-500 hover:cursor-pointer font-title">Services</RouterLink>
                <!-- <li class="hover:text-green-500 hover:cursor-pointer font-title">About Us</li>
                <li class="hover:text-green-500 hover:cursor-pointer font-title">Services</li> -->
            </ul>
            <button class="bg-green-500 p-3 rounded text-white font-title">Get a Qoute</button>
        </div>
    </nav>
</template>


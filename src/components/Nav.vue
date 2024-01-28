<script setup>

</script>

<template>
  <nav class="flex flex-col items-center lg:items-start lg:flex-row lg:justify-between p-1 mt-3 w-full">
    <div class="lg:ml-20 items-center">
      <img src="../assets/logo.jpg" alt="" width="80" >
    </div>
    <div class="flex items-center space-x-6 lg:mr-20">
      <ul class="flex lg:space-x-8 space-x-3 items-center text-lg">
        <RouterLink to="/" class="hover:text-green-500 hover:cursor-pointer font-title">Home</RouterLink>
        <RouterLink to="/about" class="hover:text-green-500 hover:cursor-pointer font-title truncate">About Us</RouterLink>
        <RouterLink to="/services" class="hover:text-green-500 hover:cursor-pointer font-title">Services</RouterLink>
        <RouterLink to="/contact" class="hover:cursor-pointer font-title bg-green-500 p-3 text-white rounded text-sm truncate">Get a Qoute</RouterLink>
      </ul>
    </div>
  </nav>
</template>
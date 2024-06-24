<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue';
import Nav from './components/Nav.vue';
import { RouterView } from 'vue-router'
</script>

<template>
  <Header/>
  <Nav/>
  <RouterView/>
  <Footer/>
</template>

<style scoped>
</style>

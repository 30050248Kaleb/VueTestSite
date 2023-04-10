<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
</script>

<template>
  <h1 class="display-5">Vue Site</h1>
  <Navbar />
  <RouterView />
</template>

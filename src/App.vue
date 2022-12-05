<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
</script>

<template>
  <div class="big-appplication is-family-primary	">
    <Navbar></Navbar>
  <section class="hero is-fullheight-with-navbar">
    <div class="hero-body">
      <RouterView />
    </div>
  </section>
  </div>
 

</template>

<style scoped>

</style>

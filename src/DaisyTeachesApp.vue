<script setup lang="ts">
import { RouterView } from 'vue-router'
import Header from './components/DaisyTeachesHeader.vue'
import Footer from './components/DaisyTeachesFooter.vue'
</script>

<template>
  <header>
    <Header></Header>
  </header>

  <RouterView />

  <footer>
    <Footer></Footer>
  </footer>
</template>

<style scoped></style>

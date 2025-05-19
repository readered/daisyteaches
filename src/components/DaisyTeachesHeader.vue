<template>
  <div class="bg-black h-20 md:h-30">
    <div class="absolute left-0 h-full mt-2 md:mt-6">
      <daisy-teaches-menu class=""></daisy-teaches-menu>
    </div>

    <div class="h-full grid justify-center content-center">
      <div class="text-white text-2xl md:text-4xl">
        <a href="/" class="flex items-center">
          <img src="../assets/daisy-flower.png" alt="Daisy" class="h-10 m-3">
          <span>Daisy Teaches</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import DaisyTeachesMenu from './DaisyTeachesMenu.vue'
</script>

<style scoped></style>

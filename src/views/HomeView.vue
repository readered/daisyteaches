<script setup lang="ts">
const buttonClasses = ["rounded-md", "border", "text-center", "text-3xl", "p-5", "border-2 border-stone-600 text-stone-600 font-medium rounded-lg hover:bg-stone-200 transition duration-300"]
</script>

<template>
  <main class="md:mt-50 md:mx-20 mx-10 mt-10">
    <h1 class="md:text-[8rem] text-[5rem]">Daisy Teaches</h1>
    <h3 class="md:text-[3rem] text-[2rem]">Bespoke, impactful and engaging English tutoring for students 11-18</h3>
    <div class="w-full grid md:grid-cols-3 grid-cols-1 gap-5 mt-10">
      <a href="/services" :class="buttonClasses">Services</a>
      <a href="/about" :class="buttonClasses">About</a>
      <a href="/testimonials" :class="buttonClasses">Testimonials</a>
    </div>
  </main>
</template>

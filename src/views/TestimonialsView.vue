<template>
  <div>
    <page-header>Testimonials</page-header>
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-10 mx-10 lg:mx-[15%] mb-10">
      <div v-for="testimonial in testimonials" :key="testimonial.quote" class="border-l-5 p-5">
        <div class="text-3xl mb-5">"{{ testimonial.quote }}"</div>
        <div class="italic">{{ testimonial.by }}</div>
      </div>
    </div>
    <div class="w-full flex justify-center mb-30">
      <link-button link="/contact">Contact Me</link-button>
    </div>
  </div>
</template>

<script setup lang="ts">
import PageHeader from '../components/PageHeader.vue'
import LinkButton from '../components/LinkButton.vue'

const testimonials = [
  {
    quote: "She now has a greater understanding of what is required for the highest grades – we only wish we had found you sooner…",
    by: "Parent of year 11 student"
  },
  {
    quote: "From only getting a 2 and a 3 in the mocks, for my GCSE results I managed to get a 7 in Language and an 8 in Literature.",
    by: "Year 11 student"
  },
  {
    quote: "You have certainly made him fall in love with English and that’s like winning the lottery for me!",
    by: "Parent of a year 9 student"
  },
  {
    quote: "I went from hating English to enjoying studying it in my spare time..!",
    by: "Year 11 student"
  },
  {
    quote: "You are so enthusiastic, fun and have so much patience!",
    by: "Parent of a year 11 student"
  }
]

</script>

<style scoped></style>

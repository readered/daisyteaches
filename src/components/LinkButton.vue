<template>
  <a :href="props.link" :class="buttonClasses">{{ props.text }}<slot></slot></a>
</template>

<script setup lang="ts">
const buttonClasses = ["rounded-md", "border", "text-center", "text-xl md:text-2xl", "py-5 px-10", "border-2 border-stone-600 text-stone-600 font-medium rounded-lg hover:bg-stone-200 transition duration-300"]

const props = defineProps(['link', 'text'])

</script>

<style scoped></style>

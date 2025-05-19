<template>
  <div>
    <div class="p-5">
      <button :class="['burger-btn text-xs md:text-sm', isOpen ? 'active' : '']" aria-label="Menu"
        @click="isOpen = !isOpen">
        <span class="burger-line"></span>
        <span class="burger-line"></span>
        <span class="burger-line"></span>
      </button>
    </div>
    <div :class="['fixed left-0 h-dvh w-full md:w-1/2 lg:w-/1/4 bg-black text-white pl-5', isOpen ? '' : 'hidden']">
      <template v-for="l in links" :key="l.link">
        <a class="block py-3 text-4xl" :href="l.link">{{ l.text }}</a>
      </template>

    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const isOpen = ref(false)
const links = [
  {
    link: '/',
    text: 'Home'
  }, {
    link: '/about',
    text: 'About'
  }, {
    link: '/services',
    text: 'Services'
  }, {
    link: '/testimonials',
    text: 'Testimonials'
  }, {
    link: '/contact',
    text: 'Contact'
  }
]

</script>

<style scoped>
.burger-btn {
  width: 2.5em;
  height: 1.8em;
  position: relative;
  background: transparent;
  border: none;
  cursor: pointer;
  padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.burger-line {
  display: block;
  width: 100%;
  height: 0.25em;
  background: white;
  border-radius: 0.125em;
  transition: all 0.3s ease;
}

/* Optional animation when clicked */
.burger-btn.active .burger-line:nth-child(1) {
  transform: translateY(0.8em) rotate(45deg);
}

.burger-btn.active .burger-line:nth-child(2) {
  opacity: 0;
}

.burger-btn.active .burger-line:nth-child(3) {
  transform: translateY(-0.8em) rotate(-45deg);
}
</style>

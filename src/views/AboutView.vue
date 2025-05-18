<template>
  <div class="">
    <page-header>About</page-header>
    <div class="mt-5 mx-5 lg:mx-[20%] grid grid-cols-4">
      <div>
        <img class="rounded-2xl w-full" src="../assets/daisy-profile-edited.jpg" alt="Daisy Teaches">
      </div>
      <div class="col-span-3 px-10 pt-5">
        <p>I am a fully qualified English teacher with over 9 years of teaching experience, working with students across
          KS3, KS4 & KS5. I originally began tutoring alongside my full-time teaching job in 2019, and have since
          garnered extensive experience tutoring both individuals and groups in an online setting.</p>
        <p>I have taught a variety of GCSE exam boards including AQA & Eduqas, and am an experienced teacher of A Level
          Literature and Lang/Lit.</p>
        <p>I have worked successfully with students of all abilities, from those working towards that all-important pass
          at GCSE to those seeking a final push towards a grade 9, or a top A Level result. I also have extensive
          experience of working with students with SEN.</p>
        <p>As a teacher & tutor I pride myself on delivering knowledge-rich, highly impactful and personalised sessions
          – with a sense of humour and an engaging approach.</p>
        <p>Daisy Teaches was born in 2022 and is run from my home in Cornwall, where I live with my husband and two
          children.</p>
        <p>I would love to hear from you with any enquiries, and am always happy to chat with prospective tutees and
          their parents or guardians to discuss how I can help them achieve their goals, or advise what style of
          tutoring might be best for them.</p>
        <p>English BA (Hons) 2.1 – Warwick University (2014)</p>
        <p>PGCE Secondary English – Roehampton University (2016)</p>
      </div>
    </div>
    <div class="w-full flex justify-center mb-30">
      <link-button link="/contact">Contact Me</link-button>
    </div>
  </div>
</template>

<script lang="ts" setup>

import PageHeader from '../components/PageHeader.vue'
import LinkButton from '../components/LinkButton.vue'

</script>

<style scoped>
p {
  font-size: 1.4rem;
  margin-bottom: 2rem;
  font-family: Jost, sans-serif;
  font-weight: lighter;
}
</style>

<template>
  <div>

    <section class="mx-10 lg:mx-[25%] my-10">
      <div class="">
        <h2 class="text-3xl">Get in Touch</h2>
        <p class="text-xl mt-5">
          Fill out the form below and I'll get back to you as soon as possible.
        </p>
      </div>

      <form class="" action="https://api.web3forms.com/submit" method="POST">

        <input type="hidden" name="access_key" value="887a5787-0eb8-474a-8724-10b22e44361b" />
        <input type="hidden" name="subject" value="New Contact Form Submission from Daisy Teaches" />
        <input type="hidden" name="from_name" value="Daisy Teaches" />
        <!-- More custom ization options available in the docs: https://docs.web3forms.com -->

        <div class="">
          <div :class="formGroupClasses">
            <label for="name" :class="labelClasses">Name</label>
            <input id="name" name="name" :class="inputClasses" placeholder="Your name" type="text" />
          </div>
          <div :class="formGroupClasses">
            <label for="email" :class="labelClasses">Email</label>
            <input id="email" name="email" :class="inputClasses" placeholder="Your email" type="email" />
          </div>
          <!-- <div class="form-group">
            <label for="phone" class="form-label">Phone</label>
            <input id="phone" name="phone" class="form-input" placeholder="" type="text" />
          </div> -->
          <div :class="formGroupClasses">
            <label for="message" :class="labelClasses">Message</label>
            <textarea :class="inputClasses" id="message" name="message" placeholder="Your message" rows="5"></textarea>
          </div>
        </div>
        <div class="w-full flex justify-end mb-30">
          <button
            class="cursor-pointer border-2 border-stone-400 hover:border-stone-600 focus:border-stone-600 hover:bg-stone-200 transition duration-300 rounded py-3 px-6"
            type="submit">Send Message</button>
        </div>

      </form>

    </section>
  </div>
</template>

<script setup lang="ts">
const formGroupClasses = ['my-5']
const labelClasses = ['block', 'mb-2']
const inputClasses = ['outline-2 outline-offset-2 outline-slate-200 rounded w-full p-1 focus:outline-stone-600 hover:outline-stone-300']

</script>

<style scoped></style>

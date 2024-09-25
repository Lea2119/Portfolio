<script setup lang="ts"></script>

<template>
  <div class="about d-flex flex-column">
    <v-card class="ma-4 pa-4" variant="text" style="line-height: 2.5">
      <p class="gradient-text text-h2 pb-4 font-weight-bold">Get in Touch</p>
      <p class="pt-4 text-justify">
        I’m always excited to connect with fellow developers, creatives, and collaborators! Whether
        you have a project in mind, want to chat about development, or are simply curious about my
        work, feel free to reach out. I’m open to new opportunities, or just a friendly conversation
        about web development and design. Looking forward to hearing from you!
      </p>
      <v-list class="pt-4">
        <ContactLink href="mailto:lea.csgn@gmail.com" text="Mail" />
        <ContactLink href="https://github.com/Lea2119" text="GitHub" />
        <ContactLink
          href="https://www.linkedin.com/in/l%C3%A9a-cassegrain-arbe-9b4b1b270/"
          text="LinkedIn"
        />
      </v-list>
    </v-card>
  </div>
</template>

<script setup lang="ts">
import ContactLink from '@/components/ContactLink.vue'
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
  }
}
.gradient-text {
  background: linear-gradient(to right, #ff7e5f, #feb47b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

<script setup lang="ts"></script>

<template>
  <div class="about d-flex flex-column">
    <v-card class="ma-4 pa-4" variant="text" style="line-height: 2.5">
      <p class="gradient-text text-h2 pb-4 font-weight-bold">About me</p>
      <p class="pt-4 text-justify">
        Before transitioning into software development, I spent several years as a registrar in the
        art market, where I oversaw the logistics of shipping artworks for clients, fairs, and
        exhibitions. This role allowed me to sharpen my organizational, self-management, and
        teamwork skills, while emphasizing the importance of clear communication and the ability to
        adapt to unforeseen challenges.
        <v-spacer></v-spacer>
        <br />
        Driven by my passion for creativity and technology, I decided to pursue web development
        through a specialized training program. During this time, I gained hands-on experience
        building projects with Vue, React, JavaScript, and TypeScript, and I am eager to bring these
        skills to a collaborative and innovative team. My expertise also includes practical
        experience with Vue.js (both Vue 2 and Vue 3), Vuetify, Pinia, and TypeScript. I focus on
        developing responsive, user-friendly web applications, maintaining high code quality through
        testing, and thriving within Agile environments.
        <v-spacer></v-spacer>
        <br />
        Outside of coding, I have a strong interest in 3D design and am currently learning Blender
        (creating my first 3D donut was a real joy!). I also enjoy drawing on my iPad, constantly
        exploring new ways to express my creativity. I am committed to continuous learning and
        personal growth as a developer, and I am excited to contribute to impactful projects by
        delivering reliable and effective solutions.
      </p>
    </v-card>
  </div>
</template>

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

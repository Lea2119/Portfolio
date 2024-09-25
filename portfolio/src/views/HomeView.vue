<template>
  <div class="px-4">
    <v-card class="ma-4 pa-4" variant="text" style="line-height: 2.5">
      <p class="gradient-text text-h2 py-2 font-weight-bold">Léa Cassegrain Arbe.</p>
      <p class="text-h2 py-2 font-weight-bold">Frontend Developer.</p>
      <div class="pt-4">
        <p>👩‍💻 Front-end Developer with hands-on experience in Vue</p>
        <p>🌟 Top Skills in TypeScript, Javascript, Vuetify, and Pinia</p>
        <p>✨ Skills in React, Django, Python and Sqlite</p>
        <p>💪 Dedicated to maintaining code quality through Test-Driven Development (TDD)</p>
        <p>🤸🏼‍♂️ Experienced in Agile workflows with a continuous learning mindset</p>
      </div>
    </v-card>
    <ProjectCard
      :image="project1"
      title="Trip Tribe"
      description="Trip Tribe is a social network designed specifically for travelers. The platform allows users to connect with fellow adventurers, share travel experiences, discover new destinations, and plan trips together. As a Web Application Developer for this project, the focus is on building a user-friendly interface and robust functionality, enabling users to easily find travel companions, create personalized itineraries, and engage with a global community of travelers."
      :technologies="[
        'TypeScript',
        'Vue',
        'Pinia',
        'Vuetify',
        'Vitest',
        'Django',
        'Python',
        'Sqlite'
      ]"
      :tools="['Git', 'GitHub', 'Figma', 'Notion', 'Slack', 'ESLint / Prettier']"
      link="https://trip-tribe-tau.vercel.app/"
    />
    <ProjectCard
      :image="project2"
      title="Curtain Call"
      description="For this project, I worked on a movie theater website that aimed to provide information about each movie currently playing and enable them to book tickets. One of the key features I implemented was the integration of video trailers, allowing users to get a glimpse of the movie. I also incorporated a Stripe component for payment transactions using credit cards."
      :technologies="['React', 'JavaScript']"
      :tools="['Git', 'GitHub', 'Figma', 'ESLint / Prettier']"
      link="https://curtain-call.vercel.app/"
    />
    <ProjectCard
      :image="project3"
      title="Cornerstore Club"
      description="I built a website where users can buy credits to access gym classes. I created offers for the credits and implemented a booking system for users to reserve classes at specified times."
      :technologies="['React', 'JavaScript']"
      :tools="['Git', 'GitHub', 'Figma', 'ESLint / Prettier']"
      link="https://cornerstore-club.vercel.app/"
    />
  </div>
</template>

<script setup lang="ts">
import project1 from '@/assets/login6.png'
import project3 from '@/assets/cornerstore.png'
import project2 from '@/assets/curtain-call.png'
import ProjectCard from '@/components/ProjectCard.vue'
</script>

<style scoped>
.gradient-text {
  background: linear-gradient(to right, #ff7e5f, #feb47b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

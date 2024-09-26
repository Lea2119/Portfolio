<template>
  <div class="px-4">
    <v-card class="ma-4 pa-4" variant="text" style="line-height: 2.5">
      <p class="gradient-text text-h2 py-2 font-weight-bold">Léa Cassegrain Arbe</p>
      <p class="text-h2 py-2 font-weight-bold">Frontend Developer.</p>
      <p class="pt-4">
        Front-end Developer with hands-on experience in Vue.js and a solid understanding of building
        responsive web applications.Proficient in TypeScript, Vuetify, and Pinia, with a focus on
        creating user-friendly interfaces and ensuring code quality. Comfortable working in Agile
        worflow and committed to contribute to a team and improving continuously.
      </p>
    </v-card>
    <div class="ma-4 pa-4">
      <p class="gradient-text text-h2 py-2 font-weight-bold">Skills & Tools</p>
      <div class="d-flex ga-4">
        <v-card min-width="200px" variant="flat" class="pt-4">
          <v-chip-group class="pb-4 text-body-2 ga-2">
            <SkillChip
              v-for="(skill, index) in skillsGroup1"
              :key="index"
              :icon="skill.icon"
              :label="skill.label"
            />
          </v-chip-group>
          <v-chip-group class="pb-4 text-body-2 ga-2">
            <SkillChip
              v-for="(skill, index) in skillsGroup2"
              :key="index"
              :icon="skill.icon"
              :label="skill.label"
            />
          </v-chip-group>
          <v-chip-group class="pb-4 text-body-2 ga-2">
            <SkillChip
              v-for="(skill, index) in skillsGroup3"
              :key="index"
              :icon="skill.icon"
              :label="skill.label"
            />
          </v-chip-group>
        </v-card>
      </div>
    </div>
    <div class="ma-4 pa-4">
      <p class="gradient-text text-h2 py-2 font-weight-bold">Works</p>
      <ProjectCard
        :image="project1"
        title="Trip Tribe | Graduation Project"
        description="Trip Tribe is a social network designed specifically for travelers. The platform allows users to connect with fellow adventurers, share travel experiences and discover new destinations."
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
        title="Curtain Call | Personal Project"
        description="A movie theater website that provide information about movies currently playing. The platform offers an intuitive and user-friendly interface where users can book tickets."
        :technologies="['React', 'JavaScript']"
        :tools="['Git', 'GitHub', 'Figma', 'ESLint / Prettier']"
        link="https://curtain-call.vercel.app/"
      />
      <ProjectCard
        :image="project3"
        title="Cornerstore Club | Personal Project"
        description="A boxing studio website that enables users to buy credits to access classes through a booking system that helps users reserve classes at specified times."
        :technologies="['React', 'JavaScript']"
        :tools="['Git', 'GitHub', 'Figma', 'ESLint / Prettier']"
        link="https://cornerstore-club.vercel.app/"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import project1 from '@/assets/login6.png'
import project3 from '@/assets/cornerstore.png'
import project2 from '@/assets/curtain-call.png'
import SkillChip from '@/components/SkillChip.vue'
import ProjectCard from '@/components/ProjectCard.vue'

const skillsGroup1 = [
  { icon: 'mdi-vuejs', label: 'Vue' },
  { icon: 'mdi-vuetify', label: 'Vuetify' },
  { icon: '', label: 'Vitest' },
  { icon: '', label: 'Pinia' },
  { icon: 'mdi-react', label: 'React' },
  { icon: 'mdi-language-typescript', label: 'TypeScript' },
  { icon: 'mdi-language-javascript', label: 'JavaScript' }
]

const skillsGroup2 = [
  { icon: '', label: 'Django' },
  { icon: 'mdi-language-python', label: 'Python' },
  { icon: 'mdi-database', label: 'SQL' }
]

const skillsGroup3 = [
  { icon: 'mdi-git', label: 'Git' },
  { icon: 'mdi-github', label: 'GitHub' },
  { icon: 'mdi-bitbucket', label: 'Bitbucket' },
  { icon: '', label: 'Notion' },
  { icon: '', label: 'Figma' },
  { icon: 'mdi-slack', label: 'Slack' },
  { icon: '', label: 'SonarCloud' },
  { icon: '', label: 'ESLint / Prettier' }
]
</script>

<style scoped>
.gradient-text {
  background: linear-gradient(to right, #ff7e5f, #feb47b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

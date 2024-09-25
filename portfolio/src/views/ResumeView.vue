<template>
  <div class="about d-flex flex-column ma-4 pa-4">
    <p class="gradient-text text-h2 pb-4 font-weight-bold">Resume</p>
    <v-tabs v-model="tab" color="#ff7e5f">
      <v-tab value="one">SP</v-tab>
      <v-tab value="two">EN</v-tab>
    </v-tabs>
    <v-card-text>
      <v-tabs-window v-model="tab">
        <v-tabs-window-item value="one">
          <v-img width="1000" height="1500" :src="resume1" />
        </v-tabs-window-item>
        <v-tabs-window-item value="two">
          <v-img width="1000" height="1500" :src="resume2" />
        </v-tabs-window-item>
      </v-tabs-window>
    </v-card-text>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import resume1 from '@/assets/resume-spa.png'
import resume2 from '@/assets/resume-en.png'

const tab = ref('one')
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

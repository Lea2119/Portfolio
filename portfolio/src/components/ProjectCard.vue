<template>
  <v-card class="ma-8 pa-4" variant="flat">
    <div class="d-flex justify-space-between">
      <div class="flex-grow-1" rounded="0" max-width="50%">
        <v-img aspect-ratio="16/9" cover height="400" :src="image"></v-img>
      </div>
      <div style="max-width: 50%" class="px-4">
        <p class="text-h4 font-weight-bold pb-4 gradient-text">{{ title }}</p>
        <p class="flex-wrap text-justify pb-4 text-body-2" style="line-height: 2.5">
          {{ description }}
        </p>
        <v-chip-group class="pb-4 text-body-2 ga-2">
          <v-chip v-for="(tech, index) in technologies" :key="index" label>{{ tech }}</v-chip>
        </v-chip-group>
        <v-chip-group class="pb-4 text-body-2 ga-2">
          <v-chip v-for="(tool, index) in tools" :key="index" label>{{ tool }}</v-chip>
        </v-chip-group>
        <v-card-actions class="pa-0">
          <a :href="link" target="_blank" style="text-decoration: none; color: inherit">
            <v-btn
              variant="flat"
              color="black"
              class="text-uppercase"
              append-icon="mdi-open-in-new"
              text="Go to site"
            />
          </a>
        </v-card-actions>
      </div>
    </div>
  </v-card>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  image: String,
  title: String,
  description: String,
  technologies: Array,
  tools: Array,
  link: String
})
</script>

<style scoped>
.gradient-text {
  background: linear-gradient(to right, #ff7e5f, #feb47b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

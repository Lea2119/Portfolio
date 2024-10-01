<template>
  <div id="home">
    <v-layout class="d-flex justify-center align-center">
      <v-app-bar class="px-2" flat>
        <div class="d-flex justify-center align-center flex-column">
          <v-img :width="150" class="text-center ma-4" />
        </div>
        <template v-slot:append>
          <v-btn to="/" text="Work" variant="text" class="mr-4" />
          <v-btn to="/about" text="About" variant="text" />
          <v-btn to="/contact" text="Contact" variant="text" />
        </template>
      </v-app-bar>
      <v-main class="main">
        <router-view />
      </v-main>
    </v-layout>
  </div>
</template>

<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<style scoped>
#home {
  background-color: white;
}

.main {
  width: 100vw;
  display: flex;
  justify-content: start;
  align-items: start;
}
</style>

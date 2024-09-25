<template>
  <v-list-item-action>
    <a :href="href" target="_blank" style="text-decoration: none; color: inherit">
      <p class="text-h2 py-2">{{ text }}</p>
    </a>
  </v-list-item-action>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  href: String,
  text: String
})
</script>

<style scoped></style>

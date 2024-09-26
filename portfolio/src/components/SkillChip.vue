<template>
  <v-chip :prepend-icon="icon" label>{{ label }}</v-chip>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  icon: String,
  label: String
})
</script>

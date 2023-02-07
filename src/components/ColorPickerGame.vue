<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script setup>
import { useColor } from '../composables/color-picker.js'

const { colors, message, matchColor }  = useColor()
</script>

<style></style>

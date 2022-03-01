<template>
  <button class="bg-red-300 m-4 p-4 rounded text-lg" @click="greet()">
    🦀 + 🕸 Hello WebAssembly!
  </button>
</template>

<script setup lang="ts">
import init, { greet } from 'wasm'

init()
</script>

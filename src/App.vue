<script setup>
import { ref } from 'vue';

const isDisabled = ref(true);
</script>

<template>
  <div>
    <!-- TODO:Teleport -->
    <button @click="isDisabled = !isDisabled">移動</button>
    <teleport to=".box" :disabled="isDisabled">
      <p>移動我到 box</p>
    </teleport>
  </div>
</template>

<style scoped></style>

<script setup lang="ts">
import { ref } from 'vue'
const color = ref<string>("#042995")
</script>

<template>
  <input id="color-input" type="text" v-model="color" placeholder="Input color string" autofocus="true"
    :style="{ backgroundColor: color }" />
</template>

<style>
#color-input {
  border: none;
  height: 100%;
  width: 100%;
  background: none;
  text-align: center;
  padding: 0;
  margin: 0;
  font-size: 48px;
}

#color-input::placeholder {
  color: black;
}

#color-input:focus-visible {
  outline: none;
}
</style>
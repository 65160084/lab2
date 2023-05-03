<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import CalComponent from './components/CalComponent.vue';
import HelloWorldExample from './components/HelloWorldExample.vue';
import HandlingUserInput from './components/HandlingUserInput.vue';
</script>

<template>
  <div>
    <HandlingUserInput />
    <CalComponent />
    <HelloWorldExample />
  </div>
</template>

<style scoped>
</style>

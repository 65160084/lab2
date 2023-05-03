<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import CalComponent from './components/CalComponent.vue';
import HelloWorldExample from './components/HelloWorldExample.vue';
import HandlingUserInput from './components/HandlingUserInput.vue';
import AttributeBindings from './components/AttributeBindings.vue';
</script>

<template>
  <div>
    <AttributeBindings />
    <HandlingUserInput />
    <CalComponent />
    <HelloWorldExample />
  </div>
</template>

<style scoped>
</style>

<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import CalComponent from './components/CalComponent.vue';
import HelloWorldExample from './components/HelloWorldExample.vue';
import HandlingUserInput from './components/HandlingUserInput.vue';
import AttributeBindings from './components/AttributeBindings.vue';
import ConditionsAndLoops from './components/ConditionsAndLoops.vue';
</script>

<template>
  <div>
    <ConditionsAndLoops />
    <br />
    <br />
    <AttributeBindings />
    <HandlingUserInput />
    <CalComponent />
    <HelloWorldExample />
  </div>
</template>

<style scoped>
</style>

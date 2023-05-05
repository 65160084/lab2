<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import CalComponent from './components/CalComponent.vue';
import HelloWorldExample from './components/HelloWorldExample.vue';
import HandlingUserInput from './components/HandlingUserInput.vue';
import AttributeBindings from './components/AttributeBindings.vue';
import ConditionsAndLoops from './components/ConditionsAndLoops.vue';
import FormBindings from './components/FormBindings.vue';
import SimpleComponent from './components/SimpleComponent.vue';
</script>

<template>
  <div>
    <SimpleComponent />
    <br />
    <br />
    <FormBindings />
    <br />
    <br />
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

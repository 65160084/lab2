<script setup lang="ts">
import {ref} from 'vue';
const message = ref("Hello world!");
function reverseMessage() {
    message.value = message.value.split("").reverse().join("");
}
function notify() {
    alert("Navigation was prevented.");
}
</script>

<template>
    <h1>{{ message }}</h1>
    <button @click="reverseMessage">Reverse Messgae</button>
    <button v-on:click="message += '!'">Append "!"</button>
    <a href="้https://vusjs.org" @click.prevent="notify">A link with e.prevendDefault</a>
</template>

<style scoped>
button, a{
  display: block;
  margin-bottom: 1em;
}
</style>
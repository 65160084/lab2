<script setup lang="ts">
import {ref} from 'vue';
import TodoItem from './TodoItem.vue';
const grocerylist = ref([
    { id: 0, text: "Vegatables" },
    { id: 1, text: "Cheese" },
    { id: 2, text: "Whatever else humans are supposed to eat" }
]);
</script>

<template>
    <ol>
        <TodoItem v-for="item in grocerylist" :key="item.id" :todo="item"/>   
    </ol>
</template>
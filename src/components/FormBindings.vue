<script setup lang="ts">
import {ref} from 'vue';
const text = ref("Edit me")
const checked = ref(true);
const checkedNames = ref(["Jack"]);
const picked = ref();
const selected = ref();
const multiSelected = ref([]);
</script>

<template>
    <h2>Text input</h2>
    <input v-model="text"/>{{ text }}

    <h2>Checkbox</h2>
    <input type="checkbox" v-model="checked" id="checkbox"/>
    <label for="checkbox">check: {{ checked }}</label>

    <h2>Multiple Checkbox</h2>
    <input type="checkbox" v-model="checkedNames" id="jack" value="Jack"/>
    <label for="jack">Jack</label>
    <input type="checkbox" v-model="checkedNames" id="john" value="John"/>
    <label for="john">John</label>
    <input type="checkbox" v-model="checkedNames" id="mick" value="Mick"/>
    <label for="mick">Mick</label>
    <p>Check names</p>
    <pre>{{ checkedNames }}</pre>

    <h2>Radio</h2>
    <input type="radio" v-model="picked" id="one" value="One"/>
    <Label for="one">One</Label>
    <input type="radio" v-model="picked" id="two" value="Two"/>
    <Label for="two">Two</Label><br/>
    <span>Picked: {{ picked }}</span>

    <h2>Select</h2>
    <select v-model="selected">
    <option disabled>Please select one</option>
        <option value="1">A</option>
        <option value="2">B</option>
        <option value="3">C</option>
    </select>
    <span>Selected: {{ selected }}</span>

    <h2>Multiple Select</h2>
    <select v-model="multiSelected" multiple style="width: 100px;">
    <option disabled>Please select one</option>
        <option value="1">A</option>
        <option value="2">B</option>
        <option value="3">C</option>
    </select>
    <span>Selected: {{ multiSelected }}</span>
</template>

<script scoped>
</script>
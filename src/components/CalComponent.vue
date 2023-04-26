<script setup lang="ts">
import {reactive, computed} from 'vue'
const state = reactive({
        num1: '0',
        num2: '0',
        result: 0
    })
    const result = computed(function() {
        return parseInt(state.num1) + parseInt(state.num2)
    })
    const doAdd = function() {
        state.result = parseInt(state.num1) + parseInt(state.num2)
    }
            
</script>

<template>
    <div class="card">
                <div>
                    <input
                        v-model="state.num1"
                        type="text"
                        ref="num1"
                        style="text-align: center; width: 80%"
                    />
                </div>
                <div>+</div>
                <div>
                    <input
                        v-model="state.num2"
                        type="text"
                        ref="num2"
                        style="text-align: center; width: 80%"
                    />
                </div>
                <hr />
                <button @click="doAdd()" style="width: 80%">=</button>
                <div ref="result">{{state.num1}}+{{state.num2}} = {{result}}</div>
            </div>
</template>

<style>
  .center_text {
            text-align: center;
            font-size: 20pt;
            margin: 5px;
        }
  .bold_text{
            font-weight:  bolder;
        }
  .card {
            padding: 10px;
            border-style: dashed;
            width: 400px;
            text-align: center;
        }
  .w100px{
            width: 100px;
        }
</style>
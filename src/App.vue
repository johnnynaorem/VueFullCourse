<template>
  <h1>CheckBox</h1>
  <div>Checked Names: {{ checkNames }}</div>
  <input type="checkbox" id="john" v-model="checkNames" value="John" />
  <label for="john">John</label>
  <input type="checkbox" id="johnny" v-model="checkNames" value="Johnny" />
  <label for="johnny">Johnny</label>
  <input type="checkbox" id="rishi" v-model="checkNames" value="rishi" />
  <label for="rishi">Rishi</label>

  <h1>Radio</h1>
  <div>Picked: {{ picked }}</div>
  <input type="radio" id="one" v-model="picked" value="One" />
  <label for="one">One</label>
  <input type="radio" id="two" v-model="picked" value="Two" />
  <label for="two">Two</label>

  <h1>Select</h1>
  <div>Selected: {{ selected }}</div>
  <select v-model="selected" multiple>
    <option>1</option>
    <option>2</option>
    <option>3</option>
  </select>
</template>

<script setup>
import { ref } from 'vue';

const checkNames = ref([]);
const picked = ref('');
const selected = ref()

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

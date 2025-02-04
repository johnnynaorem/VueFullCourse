<template>
  <div>Checked Names: {{ checkNames }}</div>
  <input type="checkbox" id="john" v-model="checkNames" value="John" />
  <label for="john">John</label>
  <input type="checkbox" id="johnny" v-model="checkNames" value="Johnny" />
  <label for="johnny">Johnny</label>
  <input type="checkbox" id="rishi" v-model="checkNames" value="rishi" />
  <label for="rishi">Rishi</label>
</template>

<script setup>
import { ref } from 'vue';

const checkNames = ref([]);

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

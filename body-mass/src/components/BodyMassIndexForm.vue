<script setup>


const emit = defineEmits("stats-entered");
</script>

<template>
  <div>
    <label for="height">Height in meters </label> <!-- height input label-->
    <input id="height" v-model="stats" /><!-- height input -->
  </div>
  <div>
    <label for="weight">Weight in kilograms </label> <!-- weight input label-->
    <input id="weight" v-model="stats" /> <!-- weight input label-->
  </div>

    <button v-on:click="emit('stats-entered',[weight, height])">Calculate</button> <!-- When button is pressed, emit so the parent can read input-->

</template>

<style scoped>
</style>

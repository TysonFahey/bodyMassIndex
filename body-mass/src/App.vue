<script setup>
import BodyMassIndexForm from "./components/BodyMassIndexForm.vue"; // import BodyMassIndexForm 

function calculate() {
    const bmi = weight / (height * height)
}
/// body mass is found by dividing weight by the height multiplied by itself
</script>

<template>
  <h1>Body Mass Index Calculator</h1> 

  <BodyMassIndexForm></BodyMassIndexForm> <!-- Display BodyMassIndexForm.vue-->

  <h2 v-on:stats-entered="calculate()">BMI is: {{bmi}}</h2> <!-- when the calulate button is pressed, call calculate function, display bmi -->

</template>

<style scoped></style>

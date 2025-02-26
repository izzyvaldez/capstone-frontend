<script setup>
import { defineEmits } from "vue";

/*
const props = defineProps({
  firstName: String,
  lastName: String,
}); 
*/

const emits = defineEmits(["greet"]);

function greetAlert() {
  emits("greet", "john doe");
}
</script>

<template>
  <!-- <h2>Hello Script Setup</h2>
  <h2>Hello {{ props.firstName }} {{ props.lastName }}</h2> -->

  <button @click="greetAlert">Greet Me</button>
</template>

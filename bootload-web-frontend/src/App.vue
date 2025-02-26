<script setup>
/*
import { ref } from "vue"; */
import GreetingMessage from "./components/GreetingMessage.vue";
import Header from "./components/Header.vue";

/*
const user = ref({
  fName: "John",
  lName: "Doe",
}); */

function greeting(name) {
  alert("Greetings! " + name);
}
</script>

<template>
  <header class="w-full bg-white shadow-md py-6 text-center">
    <h1 class="text-4xl font-bold text-gray-800">Cobbler_Pie Web Interface</h1>
  </header>
  <!-- <Header /> -->
  <!-- <GreetingMessage :firstName="user.fName" :lastName="user.lName" /> -->
  <GreetingMessage @greet="greeting" />
</template>

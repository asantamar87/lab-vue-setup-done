<template>
    <h1>New Component on Composition</h1>
    <h3>{{title}}</h3>
    <!-- <img v-bind:src="wuTangImage.image" :alt="wuTangImage.alternateText" /> -->
    <button @click="helloWorld">Iteration with Composition</button>

 <!-- Itration #03 - Creamos una funcion que nos haga display de algo en consola mediante un click event dentro del template :)  -->
  <!-- Long Version - SYNTAX -->
  <!-- <button v-on:click="wuTang()">Click me - LONG SYNTAX</button> -->

  <!-- Short Version - SYNTAX -->
  <!-- <button @click="wuTang">Click me - SHORT SYNTAX</button> -->
</template>


<script setup>
import { ref } from 'vue'

const title = ref('I am using Vue');
const helloWorld = () => {
    console.log('Hello World')
    alert( "Hello World!")
}

</script>
<style>


</style>
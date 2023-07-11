<template>
    <h2>TASK 2</h2>
    <div id="first" v-show="showBlocks">first</div>
    <div id="second" @click="clickDiv" >second</div>
    <div id="third" >third</div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  const showBlocks = ref(true);
  
  const clickDiv = () => {
    showBlocks.value = !showBlocks.value;
  };
  </script>
  
  <style scoped>
  div{
    width: 100px;
    height: 100px;
    border: 2px solid grey;
    margin: 20px;
    text-align: center;
  }
  </style>
<template>
  <h2>TASK 1</h2>
  <div id="first" @click="clickDiv">first</div>
  <div id="second" v-show="showBlocks">second</div>
  <div id="third" v-show="showBlocks">third</div>
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
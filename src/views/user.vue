<template>
  <div>
    <h1 class="text-center mt-4 mb-3">EVAL TP - Component Communication</h1>
    <div class="container bg-success p-3 rounded">
      <user-active :name="name" :age="age"></user-active>
      <user-data @update-active-user="changeData"></user-data>
    </div>
  </div>
</template>

<script setup lang='js'>

import { defineAsyncComponent, ref } from 'vue'

let name = ref('Default');
let age = ref(35);

function changeData(enteredName, enteredAge){
  name.value = enteredName;
  age.value = enteredAge;
  
}

const userData = defineAsyncComponent(()=>import("../components/userDataComp.vue"));
const userActive = defineAsyncComponent(()=>import("../components/activeUserComp.vue"));

</script>

<style scoped lang="css">

</style>
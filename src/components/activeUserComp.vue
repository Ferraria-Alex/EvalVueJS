<template>
  <div class="bg-primary-subtle text-center p-1 mb-3 rounded">
    <p class="my-2">Name: {{ props.name }}</p>
    <p class="my-2">Age: {{ props.age }} ans</p>
  </div>
</template>

<script setup lang='js'>

import {} from 'vue'

const props = defineProps({
    name:{
      type: String,
      required: true
    },
    age:{
      type: Number,
      required: true
    },
});

</script>

<style scoped lang="css">
</style>
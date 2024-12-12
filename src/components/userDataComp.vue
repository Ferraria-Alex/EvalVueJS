<template>
  <div class="d-flex flex-column p-1 bg-warning mt-2 rounded align-items-start">
    <h4 class="m-2">Formulaire d'edition :</h4>
    <input class="m-2 align-self-stretch" v-model="enteredName" type="text">
    <input class="m-2 align-self-stretch" v-model="enteredAge" type="number">
    <button class="btn btn-outline-dark m-2" @click="sendData()">Maj des Données</button>
  </div>
</template>

<script setup lang='js'>
import { ref } from 'vue'

const enteredName = ref('');
const enteredAge = ref(0);

const emit = defineEmits({
  'update-active-user': (name, age)=>{

  }
});

const sendData = () => {
  emit('update-active-user', enteredName.value, enteredAge.value);
}

</script>

<style scoped lang="css">
</style>
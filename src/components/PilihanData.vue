<template>
    <div>
      <h3>Pilihan Data</h3>
      <button @click="pilihData('Tekanan Darah')">Pilih Tekanan Darah</button>
      <button @click="pilihData('Detak Jantung')">Pilih Detak Jantung</button>
    </div>
  </template>
  
  <script setup>
  import { defineEmits } from 'vue';
  
  const emit = defineEmits(['data-dipilih']);
  
  function pilihData(data) {
    emit('data-dipilih', data);
  }
  </script>
  
<style scoped>
button {
    margin-right: 10px;
    margin-bottom: 10px;
    padding: 10px;
    border-radius: 10px;
    border: 1px solid black;
    background-color: white;
}

button:hover {
    background-color: lightgray;
    cursor: pointer;
}

</style>
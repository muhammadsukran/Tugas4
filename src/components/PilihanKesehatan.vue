<template>
    <div>
      <h2>Pilihan Kesehatan</h2>
      <PilihanData @data-dipilih="kirimData" />
    </div>
  </template>
  
  <script setup>
  import { defineEmits } from 'vue';
  import PilihanData from './PilihanData.vue';
  
  const emit = defineEmits(['data-dipilih']);
  
  function kirimData(data) {
    emit('data-dipilih', data);
  }
  </script>
  
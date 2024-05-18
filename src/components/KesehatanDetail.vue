<template>
    <div>
      <h1>Detail Kesehatan</h1>
      <p>Data yang Dipilih: {{ dataTerpilih }}</p>
      <PilihanKesehatan @data-dipilih="perbaruiData" />
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  import PilihanKesehatan from './PilihanKesehatan.vue';
  
  const dataTerpilih = ref(null);
  
  function perbaruiData(data) {
    dataTerpilih.value = data;
  }
  </script>
  
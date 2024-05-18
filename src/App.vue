<template>
  <body>
  <div id="app" class="app">
    <KesehatanDetail />
  </div>
</body>
</template>

<script setup>
import KesehatanDetail from './components/KesehatanDetail.vue';
</script>

<style>
@keyframes border {
  0% {
    border-image-source: linear-gradient(10deg, rgb(42, 40, 59), transparent, rgb(3, 41, 46),transparent, rgb(42, 40, 59));
    border-image-slice: 1;
    box-shadow: 0 0 30px whitesmoke;
  }
  50%{
    border-image-source: linear-gradient(100deg, rgb(112, 126, 248), transparent, rgb(37, 91, 2), transparent, rgb(152, 190, 90));
    border-image-slice: 1;
    box-shadow: 0 0 40px whitesmoke;
  }
  100% {
    border-image-source: linear-gradient(360deg,rgb(42, 40, 59), transparent, rgb(3, 41, 46),transparent, rgb(42, 40, 59));
    border-image-slice: 1;
    box-shadow: 0 0 50px whitesmoke;
  }
}

#app {
  position: fixed;
  left: 40%;
  top: 20%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  text-shadow: 0 0 1px wheat;
}

.app {
  padding: 20px 20px;
  border: 5px solid;
  border-radius: 20px;
  border-image-slice: 1;
  animation: border 3s cubic-bezier(0.68, -0.55, 0.27, 1.55) infinite;
}

body {
  background-color: black;
}
</style>

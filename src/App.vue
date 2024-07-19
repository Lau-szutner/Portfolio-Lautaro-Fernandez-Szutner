<script setup>
import Navbar from "./components/Navbar.vue";
import Home from "./components/Home.vue";
// import TrianglePattern from "./components/TrianglePattern.vue";

// Importar el CSS de forma estándar
import "./assets/css/normalize.css";
</script>

<template>
  <Navbar></Navbar>
  <img src="./assets/img/Header.png" alt="" />
  <!-- <TrianglePattern></TrianglePattern> -->
  <Home></Home>
</template>

<style scoped>
img {
  width: 100vw;
  height: 100%;
}
</style>

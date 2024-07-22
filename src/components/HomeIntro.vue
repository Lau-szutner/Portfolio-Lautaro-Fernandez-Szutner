<template>
  <section class="home-intro">
    <div
      class="d-flex flex-column justify-content-center align-items-center vh-100 col-6 d-block"
    >
      <h1>
        <span>Lautaro</span>
        <span>Fernandez</span>
        <span>Szutner</span>
      </h1>
      <p>{{ introduction }}</p>
    </div>
    <img src="../assets/img/Header.png" alt="" class="" />
  </section>
</template>

<script setup>
import { ref } from "vue";

const introduction = ref("Diseñador & Programador web");
</script>

<style scoped>
.home-intro {
  text-align: center;
}
.home-intro h1 {
  font-family: "Montserrat", sans-serif;
  font-optical-sizing: auto;
  font-weight: 700;
  font-size: 4em;
  font-style: italic;
  color: rgb(0, 129, 241);
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.home-intro p {
  font-family: "Montserrat", sans-serif;
  font-optical-sizing: auto;
  font-weight: 700;
  font-style: italic;
  font-size: 1.25rem;
  color: #ec0a0a;
  margin-bottom: 0px;
  display: flex;
}

img {
  width: 100vw;
  height: 100%;
}
section {
  display: flex;
  flex-direction: row;
}
img {
  position: absolute;
  z-index: -1;
}
</style>

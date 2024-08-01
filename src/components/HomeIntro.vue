<template>
  <section class="home-intro">
    <div
      class="d-flex flex-column justify-content-center align-items-center vh-100 col-6"
    >
      <h1 class="d-flex flex-column align-items-start">
        <span>Lautaro</span>
        <span>Fernandez</span>
        <span>Szutner</span>
      </h1>
      <div class="d-flex flex-column align-items-start w-50">
        <p>Diseñador</p>
        <p>& Programador web</p>
      </div>
    </div>
    <img src="../assets/img/background.png" alt="" class="" />
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
  color: var(--header-color);
}
.home-intro p {
  font-family: "Montserrat", sans-serif;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: italic;
  font-size: 2rem;
  color: var(--text-color);
  margin-bottom: 0px;
}

img {
  height: fit-content;
  width: 100%;
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

<script setup></script>

<template>
  <div id="contenedor" class="container-fluid">
    <header class="d-flex justify-content-center py-3">
      <ul class="nav nav-pills gap-5">
        <li class="nav-item">
          <a href="#" class="nav-link smooth-link" aria-current="page"
            >Inicio</a
          >
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link smooth-link">Quién soy</a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link smooth-link">Proyectos</a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link smooth-link">Habilidades</a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link smooth-link">Contacto</a>
        </li>
      </ul>
    </header>
  </div>
</template>

<style lang="scss" scoped>
#contenedor {
  background-color: black;
}

li {
  font-family: "Montserrat", sans-serif;
  font-optical-sizing: auto;
  font-style: normal;
  color: white;
  font-size: 2em;
  font-weight: 300;
}

.smooth-link {
  position: relative;
  color: white;
  cursor: pointer; /* Opcional: para cambiar el cursor al estilo de un enlace */
  transition: color 0.3s ease; /* Transición para el color del texto */
}

.smooth-link::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -2px; /* Ajusta la posición vertical de la línea */
  width: 100%;
  height: 1px; /* Ajusta el grosor de la línea */
  background: var(--header-color); /* Color de la línea */
  transition: transform 0.3s ease; /* Transición para la línea */
  transform: scaleX(0);
  transform-origin: bottom right; /* Inicia la animación desde la derecha */
}

.smooth-link:hover::after {
  transform: scaleX(1); /* Hace que la línea se expanda completamente */
  transform-origin: bottom left; /* Anima hacia la izquierda */
}

.smooth-link:hover {
  color: var(
    --header-color
  ); /* Opcional: Cambia el color del texto al pasar el cursor */
}
</style>

---
layout: default
title: "Atelier de código"
---

[Home](/) | [Sobre nosotras](/sobre-nosotras/) | [Contacto](/contacto/)


Desde **Atelier de código** queremos acompañarte en tu camino en el análisis de datos. Para quienes quieran poner manos a la obra, dictamos **cursos** de R para principiantes (y no tan principiantes también), sobre fundamentos de la programación, limpieza y organización de datos, análisis estadísticos y visualización. Para quienes ya tienen una base pero necesitan pensar con alguien más, ofrecemos **tutorías** donde te asesoramos sobre tu análisis. Y para quienes no tengan tiempo (¡o ganas!) de aprender a programar, **analizamos** sus datos y proveemos un reporte a medida.

<style>
  .squares-container {
    display: flex;
    justify-content: space-between;
    margin: 20px;
  }

  .square {
    position: relative;
    width: 30%;
    height: 200px; /* Ajusta la altura que desees */
    perspective: 1000px; /* Para efecto de 3D */
    margin: 10px; /* Espacio entre cuadrados */
    cursor: pointer;
  }

  .square .front,
  .square .back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden; /* Ocultar el lado opuesto */
    border: 1px solid #ccc;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    transition: transform 0.6s; /* Transición suave */
  }

  .square .front {
    background-color: white; /* Color de fondo del lado frontal */
  }

  .square .back {
    background-color: #f0f0f0; /* Color de fondo del lado trasero */
    transform: rotateY(180deg); /* Darle la vuelta */
  }

  .square.flipped .front {
    transform: rotateY(180deg); /* Dar vuelta al lado frontal */
  }

  .square.flipped .back {
    transform: rotateY(0deg); /* Mostrar el lado trasero */
  }
</style>

<div class="squares-container">
  <div class="square" onclick="toggleDescription(this)">
    <div class="front">
      <h3>Cursos</h3>
    </div>
    <div class="back">
      <p>(descripción de los cursos)</p>
    </div>
  </div>
  <div class="square" onclick="toggleDescription(this)">
    <div class="front">
      <h3>Asesorías</h3>
    </div>
    <div class="back">
      <p>(descripción de las asesorías)</p>
    </div>
  </div>
  <div class="square" onclick="toggleDescription(this)">
    <div class="front">
      <h3>Análisis de datos</h3>
    </div>
    <div class="back">
      <p>(descripción del análisis de datos)</p>
    </div>
  </div>
</div>

<script>
  function toggleDescription(square) {
    square.classList.toggle('flipped'); // Alternar la clase flipped
  }
</script>

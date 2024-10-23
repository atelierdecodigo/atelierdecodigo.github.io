---
layout: default
title: "Atelier de código"
---

[Home](/) | [Sobre nosotras](/sobre-nosotras/) | [Contacto](/contacto/)


Desde **Atelier de código** queremos acompañarte en tu camino en el análisis de datos. Para quienes quieran poner manos a la obra, dictamos **cursos** de R para principiantes (y no tan principiantes también), sobre fundamentos de la programación, limpieza y organización de datos, análisis estadísticos y visualización. Para quienes ya tienen una base pero necesitan pensar con alguien más, ofrecemos **tutorías** donde te asesoramos sobre tu análisis. Y para quienes no tengan tiempo (¡o ganas!) de aprender a programar, **analizamos** sus datos y proveemos un reporte a medida.

<style>
  .squares-container {
    display: flex;
    justify-content: space-around;
    margin: 20px;
  }

  .square {
    width: 30%;
    border: 1px solid #ccc;
    border-radius: 8px;
    padding: 20px;
    text-align: center;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  .square:hover {
    background-color: #f0f0f0;
  }

  .description {
    margin-top: 10px;
    text-align: left;
  }
</style>

<div class="squares-container">
  <div class="square" onclick="toggleDescription('desc1')">
    <h3>Cursos</h3>
    <div id="desc1" class="description" style="display:none;">
      (descripción de cursos)
    </div>
  </div>
  <div class="square" onclick="toggleDescription('desc2')">
    <h3>Tutorías</h3>
    <div id="desc2" class="description" style="display:none;">
      (descripción de tutorías)
    </div>
  </div>
  <div class="square" onclick="toggleDescription('desc3')">
    <h3>Análisis de datos</h3>
    <div id="desc3" class="description" style="display:none;">
      (descripción de análisis de datos)
    </div>
  </div>
</div>

<script>
  function toggleDescription(descId) {
    var desc = document.getElementById(descId);
    if (desc.style.display === "none") {
      desc.style.display = "block";
    } else {
      desc.style.display = "none";
    }
  }
</script>


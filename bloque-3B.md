---
title: "Bloque 3:"
subtitle: >
  - Matrices en NumPy <br>
  - Trasposición, aplanamiento y reversa <br>
  - Reshape de matrices
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-3B
---

<style>
  .outer {
      width: 100%;
      max-width: 2000px;
      margin: 0 auto;
  }
  .video-wrapper {
      height: 0;
      margin: auto;
      z-index: 1;
      position: relative;
      padding-top: 25px;
      padding-bottom: 56.25%;
      display: block;
      overflow: hidden;
    
    iframe {
      display: block;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 5;
      position: absolute;
    }
  }
</style>


# Introducción a NumPy - Bloque 3

<br>
<center>
  <img width="50%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png">
</center>
<br>

En esta sección aprenderás lo básico sobre NumPy. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Matrices en NumPy
- Trasposición, aplanamiento y reversa
- Reshape de matrices

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://www.youtube.com/embed/V82s0WgW7oQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## Trasposición, aplanamiento y reversa

Es común tener que trasponer matrices. Las matrices NumPy tienen la propiedad **.T** que permite transponer una matriz. De igual manera se puede utilizar **.transpose()**

<center>
    <img src="https://numpy.org/devdocs/_images/np_transposing_reshaping.png">
</center>

En algunas ocasiones resulta útil aplanar una matriz, esto es, convertirla en un arreglo unidimensional. Esto puede lograrse con **.flatten()**

Al igual que con las listas en Python, podemos utilizar slicing para revertir un array, sin embargo, NumPy tiene una función propia: **np.flip()**

### Reshape de matrices

**.reshape()** permite cambiar la forma de una matriz sin cambiar los datos. Sólo ten presente que cuando usamos esta función, la matriz que queremos producir debe tener la misma cantidad de elementos que la matriz original.

## Matrices en NumPy

Procederemos a explorar un poco con una imagen y sus canales de color (revisar el cuaderno de trabajo).

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vTQWfTzIf5OqaIQlAN8IxYuten2qPjhhK3Tr_3R3L6NZR0EEMsFBq_kVrU8wHD5LlIA67upXC0XDWf3/pub?start=false&loop=false&delayms=3000" target="_blank">
    <img width="30%" src="https://img.shields.io/static/v1?label=Slides&message=Google%20Slides&color=tomato" alt="Google Slides"/>
  </a>
  <br><br>
  <h4>Ejecuta el código:</h4>
  <a href="https://colab.research.google.com/github/futurelabmx/cdecmx/blob/main/B%20-%20Intro%20a%20NumPy.ipynb" target="_blank">
    <img width="30%" src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
  </a>
</center>

<!-- Buttons -->
<br>
<div class="buttons has-addons is-centered">
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-2B/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-3B/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-4B/">Siguiente ▶︎</a>
</div>

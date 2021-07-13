---
title: "Bloque 3:"
subtitle: >
  - Listas y tuplas <br>
  - Ciclos
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-3A
---

# Introducción a Python - Bloque 3

<br>
<center>
  <img width="50%" src="https://www.python.org/static/community_logos/python-logo-generic.svg">
</center>
<br>

En esta sección comenzarás a trabajar con las bases de Python. Hemos preparado un video para ti, donde cubriremos los siguientes temas:

- Listas y tuplas
- Ciclos

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://youtu.be/xIbX_xWtPX8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## Colecciones

Una colección es un conjunto de elementos en una estructura de datos de Python. De manera nativa Python tiene soporte para:
- Listas y tuplas
- Diccionarios y conjuntos

```python
# Example:
my_list = [1.0, 2.0, 3.0]
my_tuple = (1.0, 2.0, 3.0)
my_dict = {
    "day": 1,
    "month": "November",
}
```

## Ciclos – `while`

Iteración significa ejecutar el mismo bloque de código una y otra vez, potencialmente muchas veces. Una estructura de programación que implementa la iteración se denomina bucle o ciclo.

Para un ciclo `while`, será importante establecer una condición de detención.

```python
# Example:
while condition:
    # Block of code
```

## Ciclos – `for`

Python tiene un ciclo basado en colecciones o en iteradores. Este tipo de ciclo itera sobre una colección de objetos, en lugar de especificar valores o condiciones numéricos, este ciclo se llama ciclo `for`.

```python
# Example:
for element in collection:
    # Block of code that iterates over a collection
```


<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vRBwP8Th2OBc_lzVnb6VPhnxCqd5PLNT7Hg8AGpxb_4ITxqeyUDoma7y_iE0Ky0mxX9VSLhX0ClbGFC/pub?start=false&loop=false&delayms=3000" target="_blank">
    <img width="30%" src="https://img.shields.io/static/v1?label=Slides&message=Google%20Slides&color=tomato" alt="Google Slides"/>
  </a>
  <br><br>
  <h4>Ejecuta el código:</h4>
  <a href="https://colab.research.google.com/github/futurelabmx/cdecmx/blob/main/A%20-%20Intro%20a%20Python.ipynb" target="_blank">
    <img width="30%" src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
  </a>
</center>

<!-- Buttons -->
<br>
<div class="buttons has-addons is-centered">
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-2A/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-3A/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-4A/">Siguiente ▶︎</a>
</div>

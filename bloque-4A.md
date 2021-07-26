---
title: "Bloque 4:"
subtitle: >
  - Diccionarios <br>
  - Funciones <br>
  - Módulos y paquetes
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-4A
---

# Introducción a Python - Bloque 4

<br>
<center>
  <img width="50%" src="https://www.python.org/static/community_logos/python-logo-generic.svg">
</center>
<br>

En esta sección comenzarás a trabajar con las bases de Python. Hemos preparado un video para ti, donde cubriremos los siguientes temas:

- Diccionarios
- Funciones
- Módulos y paquetes

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://www.youtube.com/embed/82Tko4At1Q8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## Colecciones - Diccionarios

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

## Funciones

La manera en la que empaquetamos procesos que ejecutan un bloque completo de código es a través de **funciones**, la sintaxis de Python es muy sencilla y eficiente para escribir bloques de código de forma ordenada.

La mayoría de los paquetes en Python están conformados por objetos y funciones.

```python
# Example:
def function_name(arguments):
    # Block of code
    return something
```

## Módulos y paquetes

Subiendo un nivel más de abstracción en empaquetamiento, podemos crear archivos de código (scripts) en los que podemos empaquetar funciones y objetos más robustos que nos permitan hacer procesamientos más elaborados. Estos se empaquetan en módulos que pueden importarse, y a su vez los módulos pueden agruparse en paquetes.

De manera nativa, Python ya cuenta con diversos módulos en su biblioteca estándar de funciones, que puedes consultar en la documentación oficial: [https://docs.python.org/es/3/library/index.html](https://docs.python.org/es/3/library/index.html)


<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vQCrevv0bcEW1O_oC4A8Huz2L8mEK8d50vDdYoNbGioU7C6z2CtaDVo_VumwbXWO0O99LHlycVn7wpd/pub?start=false&loop=false&delayms=3000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-3A/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-4A/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-1B/">Siguiente ▶︎</a>
</div>

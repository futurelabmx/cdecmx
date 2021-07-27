---
title: "Bloque 1:"
subtitle: >
  - Introducción a NumPy <br>
  - Atributos, tamaño y forma <br>
  - Creación de arreglos
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-1B
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


# Introducción a NumPy - Bloque 1

<br>
<center>
  <img width="50%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png">
</center>
<br>

En esta sección aprenderás lo básico sobre NumPy. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Introducción a NumPy
- Atributos, tamaño y forma
- Creación de arreglos

![YouTube Thumbnail](https://vidooly.com/blog/wp-content/uploads/2015/01/How-to-optimise-your-YouTube-Thumbnails.png)

## ¿Qué es NumPy?

**NumPy** es el paquete fundamental para la computación numérica con Python.

De acuerdo con Wikipedia: _"(...) es una biblioteca para el lenguaje de programación Python que da soporte para crear vectores y matrices grandes multidimensionales, junto con una gran colección de funciones matemáticas de alto nivel para operar con ellas."_

### Objetos en NumPy

En **NumPy**, los objetos con los que trabajamos son arreglos multidimensionales:

```
                     [1, 2, 3, 4] → [1.0 2.0 3.0 4.0]
[[1, 2, 3], [4, 5, 6], [7, 8, 9]] → [[1.0 2.0 3.0]
                                     [4.0 5.0 6.0]
                                     [7.0 8.0 9.0]]
```

### ¿Qué es un arreglo?

Un arreglo es la formalización de una lista en Python; y un array puede ser indexado por una tupla de enteros no negativos, por booleanos, por otro arreglo o por enteros. El rango de la matriz es el número de dimensiones. La forma de la matriz es una tupla de números enteros que dan el tamaño de la matriz a lo largo de cada dimensión.

Una forma en que podemos inicializar matrices NumPy es a partir de listas de Python, utilizando listas anidadas para datos bidimensionales o de mayor dimensión.

```python
a = np.array([1, 2, 3, 4, 5, 6])
a = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])

print(a[0])
# [1 2 3 4]
```

## Atributos, tamaño y forma

Un arreglo suele ser un contenedor de tamaño fijo de elementos del mismo tipo y tamaño. El número de **dimensiones** y **elementos** se define por su forma. La **forma (shape)** es una tupla de números enteros no negativos que especifican los tamaños de cada dimensión.

En NumPy, las dimensiones se denominan **ejes (axes)**.

Esto significa que si tenemos un arreglo 2D (una matriz) que se ve así:

```
[[0., 0., 0.],
 [1., 1., 1.]]
```

Entonces tenemos 2 ejes. El primer eje tiene una longitud de 2 y el segundo eje tiene una longitud de 3. (**shape=(2, 3)**)

### ¿Cómo saber la forma y tamaño?

- **ndarray.ndim** te dirá el número de ejes o dimensiones de la matriz.
- **ndarray.size** te dirá el número total de elementos de la matriz. Este es el producto de los elementos de la forma de la matriz.
- **ndarray.shape** te mostrará una tupla de números que indican el número de elementos almacenados a lo largo de cada dimensión de la matriz.

## Creación de arreglos

Además de crear un array a partir de una secuencia de elementos, puedes crear uno llena de ceros, o llena de unos:

```python
np.zeros(2)
# array([0., 0.])
np.ones(2)
# array([1., 1.])
```
<br>

También puedes usar `np.linspace()` para crear una matriz con valores espaciados linealmente en un intervalo especificado.

```python
x = np.linspace(0, 50, 51)
print(x)

y = np.sin(x)
print(y)
````

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vRKQeS9L9_8oMwgEjQF5_XXvD0GWodZpVMKH07TqSSESS6JSSl7SLJ-dXS2TFL-Dk6izFE-eUFqFZ5I/pub?start=false&loop=false&delayms=3000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-4A/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-1B/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-2B/">Siguiente ▶︎</a>
</div>

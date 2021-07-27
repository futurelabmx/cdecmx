---
title: "Bloque 2:"
subtitle: >
  - Indexación y slicing <br>
  - Operaciones básicas, broadcasting <br>
  - Valores únicos y cuentas
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-2B
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


# Introducción a NumPy - Bloque 2

<br>
<center>
  <img width="50%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png">
</center>
<br>

En esta sección aprenderás lo básico sobre NumPy. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Indexación y slicing
- Operaciones básicas, broadcasting
- Valores únicos y cuentas

![YouTube Thumbnail](https://vidooly.com/blog/wp-content/uploads/2015/01/How-to-optimise-your-YouTube-Thumbnails.png)

## Indexación y slicing

Podemos indexar y usar slicing matrices NumPy de la misma manera que hacemos con listas de Python.

```python
data = np.array([1, 2, 3])

print(data[1])
# 2
print(data[0:2])
# array([1, 2])
print(data[1:])
# array([2, 3])
print(data[-2:])
# array([2, 3])
```

La principal diferencia es que en lugar de usar múltiples corchetes, usamos comas para acceder a elementos.

## Operaciones básicas, broadcasting

Si tuviésemos un par de arrays del misma forma, podríamos operar entre ellos. Consideremos el par de arreglos a continuación:

<center>
    <img src="https://numpy.org/devdocs/_images/np_array_dataones.png">
</center>

Podríamos sumarlos:

<center>
    <img src="https://numpy.org/devdocs/_images/np_data_plus_ones.png">
</center>

```python
data = np.array([1, 2])
ones = np.ones(2, dtype=int)
print(data + ones)
# array([2, 3])
```

<br>
Esto en general se preserva para las otras operaciones básicas:

<center>
    <img src="https://numpy.org/devdocs/_images/np_sub_mult_divide.png">
</center>

```python
data - ones
# array([0, 1])

data * data
# array([1, 4])

data / data
# array([1., 1.])
```

<br>
#### ¿Qué sucede si queremos una multiplicación escalar?

## Broadcasting

<center>
    <img src="https://numpy.org/devdocs/_images/np_multiply_broadcasting.png">
</center>

```python
data = np.array([1.0, 2.0])
data * 1.6
# array([1.6, 3.2])
```

<br>
## Valores únicos y cuentas

Existen algunas funciones propias de los arreglos en NumPy:
- **.max()** te dirá el máximo de los elementos del arreglo.
- **.min()** te dirá el mínimo de los elementos del arreglo.
- **.sum()** te dirá la suma  de los elementos del arreglo.
- **.prod()** te dirá el producto de los elementos del arreglo.

Incluso existen funciones que te devuelven estadísticos de tus datos:
- **.mean()** te dirá el promedio de los elementos del arreglo.
- **.std()** te dirá la desviación estándar de los elementos del arreglo.

También puedes utilizar operaciones matemáticas básicas:
- **np.sin(x)** te devolverá el seno del vector `x`.
- **np.cos(x)** te devolverá el coseno del vector `x`
- Etcétera.

En cuanto a querer devolver valores únicos, podemos usar **.uniques()**
```python
a = np.array([11, 11, 12, 13, 14, 15, 16, 17, 12, 13, 11, 14, 18])
unique_values = np.unique(a)
print(unique_values)
# [11 12 13 14 15 16 17 18]
```

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vSbALnyMedNsW6zo6PhM7r1mH42wS-0Ou214PGYmYBCWZeUw7XBgRpOBEKCQ4c8fDfh2Bhwml-N0IEd/pub?start=false&loop=false&delayms=3000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-1B/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-2B/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-3B/">Siguiente ▶︎</a>
</div>

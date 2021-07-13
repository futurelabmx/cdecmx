---
title: "Bloque 2:"
subtitle: >
  - I/O - ¡Hola mundo! <br>
  - Variables, tipos y conversión <br>
  - Operaciones básicas <br>
  - Condicionales
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-2A
---

# Introducción a Python - Bloque 2

<br>
<center>
  <img width="50%" src="https://www.python.org/static/community_logos/python-logo-generic.svg">
</center>
<br>

En esta sección comenzarás a trabajar con las bases de Python. Hemos preparado un video para ti, donde cubriremos los siguientes temas:

- I/O - ¡Hola mundo!
- Variables, tipos y conversión
- Operaciones básicas
- Condicionales

![YouTube Thumbnail](https://vidooly.com/blog/wp-content/uploads/2015/01/How-to-optimise-your-YouTube-Thumbnails.png)

## I/O - ¡Hola mundo!

`input()` y `print()` son las funciones de entrada y salida (respectivamente) de información en Python. `input()` tiene como argumento una cadena de texto que da las instrucciones que se deseas desplegar y lo que retorna (la respuesta) siempre es una cadena de texto; mientras que print() tiene como argumentos cadenas de texto o variables que se desean desplegar.

```python
# Ejemplo:
nombre = input("Introduce tu nombre: ")
print("Mucho gusto," nombre)
```

## Variables, tipos y conversión

Podemos pensar que una variable es como un contenedor de información. Python puede albergar distintos tipos de datos, como valores numéricos, booleanos y cadenas de texto. Al ser Python de tipado dinámico, no hace falta declarar el tipo de variable, sino que sólo basta con definir sus valores.

```python
# Example:
name = "Rodolfo"
age, pi = 26, 3.1416
age = float(age)

print(name, age)
print(type(name), type(age))
```

## Operaciones básicas

En esencia hay tres tipos de operaciones:
- **Operaciones aritméticas.** Operan a nivel aritmético sobre los valores de las variables (`+, -, *, /, //, **`).
- **Operaciones de comparación.** Operan a nivel matemático sobre los valores de las variables (`<, >, <=, >=, ==, !=`).
- **Operaciones lógicas.** Operan a nivel lógico sobre las variables (`and, or, not`).

## Condicionales

Utilizaremos una **condición** para validar si se cumple uno o más estados (las condiciones) para ejecutar cierto bloque de código, en esencia nos ayuda a tomar decisiones sobre el flujo de nuestro código.

```python
# Example:
if condition:
  # Block of code
elif other_condition:
  # Another block of code
else:
  # Final block of code
```


<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vQwtnHWBOG_1qI-FnTzuqBkL3GWCHlZfD_diyTtFaHgZBnpQzCohgg_0kEu8LOUe8JNcvVx1JjN7zfP/pub?start=false&loop=false&delayms=3000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-1A/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-2A/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-3A/">Siguiente ▶︎</a>
</div>
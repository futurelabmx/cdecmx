---
title: "Bloque 1:"
subtitle: >
   - Introducción a Pandas. <br>
   - Dónde encontrar datos. <br>
   - Carga de datos de diferentes formatos. <br>
   - Series y DataFrames.
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-1C
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

# Introducción a Pandas - Bloque 1

<br>
<center>
  <img width="50%" src="https://pandas.pydata.org/docs/_static/pandas.svg">
</center>
<br>

En esta sección aprenderás lo básico sobre Pandas, al menos a un nivel conceptual. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Introducción a Pandas.
- Dónde encontrar datos.
- Carga de datos de diferentes formatos.
- Series y DataFrames.

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://www.youtube.com/embed/xm4jKcZDdxc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## ¿Qué es Pandas?
 
**Pandas** es una librería de Python con la que puedes trabajar con datos tabulados. Es muy útil para limpiar, analizar y procesar datos.
 
De acuerdo con Wikipedia: _"(...) es una biblioteca de software escrita como extensión de **NumPy** para manipulación y análisis de datos para el lenguaje de programación Python. En particular, ofrece estructuras de datos y operaciones para manipular tablas numéricas y series temporales."_
 
### Objetos en Pandas.
 
En Pandas, los objetos con los que trabajaremos son dos: **DataFrames** y Series. Un DataFrame lo puedes entender como un **tabla** (como las de Excel), y una **Series** como una **tabla con una sola columna**. Más adelante veremos mas a detalle a estos dos objetos que son los objetos base de Pandas.

## ¿Dónde encontrar datos?
 
En internet existen repositorios de **datos abiertos** de los que puedes descargar datasets, jugar con ellos, analizarlos y aprender. Algunos ejemplos:
 
1. [Kaggle](https://www.kaggle.com/datasets): Sitio web para prácticar y aprender sobre **ciencia de datos y machine learning**. Además de los datasets que hay en el sitio, ¡puedes correr notebooks como este!. Los dataset están por lo general explicados y listos para usarse.
2. [UC Irvine Machine Learning Repository](http://archive.ics.uci.edu/ml/index.php): En este repositorio hay más de **500 datasets** de diversos temas. Usualmente son útiles para practicar y aprender sobre machine learning.
3. [Datos Abiertos de México](https://datos.gob.mx/): En este sitio web se encuentra una recopilación de datos abiertos de diversas instituciones, así como del **gobierno federal y gobiernos estatales**. 
4. [INEGI](https://www.inegi.org.mx/datos/): Datos obtenidos de los diversos **censos** que realiza el Instituto Nacional de Estadística y Geografía.
 
Incluso puedes encontrar **datos abiertos de ciencia**: 
1. [CERN Opendata](https://opendata.cern.ch/): Más de dos petabytes de datos de **física de partículas**.
2. [NASA Open Data Portal](https://data.nasa.gov/): Datos aeroespaciales, de ciencias de la tierra... **¡Muchos datos!**✨
 
Esta no es una lista exhaustiva, hay muchos más recursos disponibles con los que puedes trabajar.

## Carga de datos de diferentes formatos.
 
Con Pandas puedes **cargar datos** de archivos externos, los cuales pueden estar en internet o en tu computadora (quizá bajaste alguna de las páginas de arriba 👀). Por lo general se utilizan datos tabulados (tablas) en Pandas, y los tipos de archivos desde los que puedes cargar datos son varios. Los más comunes son archivos con _valores separados por comas_ o CSV, por sus siglas en inglés, con extensión **.csv** y archivos de Excel con extensión **.xlsx**.

```python
# Para importar un archivo csv
datos = pd.read_csv('nombre_del_archivo.csv')
 
# Para importar un archivo de excel
datos = pd.read_excel('nombre_del_archivo.xlsx') 
```

<center>
    <img width="90%" src="https://pandas.pydata.org/docs/_images/02_io_readwrite.svg">
</center>
 
Hay más tipos de archivos válidos, como **.html** o **.json** y se importan al igual que los ejemplos anteriores. De la misma manera en la que cargamos datos, podemos guardar un DataFrame o una Series en un archivo con extensión válida: 
 
```python
# Guardamos los datos en un archivo CSV
datos.to_csv('datos_guardados.csv')
```

## Series y DataFrames.
 
Como ya mencionamos, una Series se puede entender como una **tabla con una sola columna**, aunque también puedes verla como una lista donde cada elemento tiene una etiqueta, un **índice** el cual por default es un número entero de la posición del elemento.
 
<center>
    <img width="12%" src="https://pandas.pydata.org/docs/_images/01_table_series.svg">
</center>

Los **DataFrames** son más complejos que las Series, ya que ahora tenemos una **tabla con varias columnas**. En este caso, tendremos **índices** para cada fila y también etiquetas para las **columnas**. Los valores default son también enteros que indican la posición.
 
<center>
    <img width="30%" src="https://pandas.pydata.org/docs/_images/01_table_dataframe.svg">
</center>

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vQ_AwnhsuerhFZIgaBePzIhwl5Z7P4zlkGpf_SdomMQBPPi0SpBeRg4TxMkwY_fOS_95-OUteYsIZ1c/pub?start=false&loop=false&delayms=60000" target="_blank">
    <img width="30%" src="https://img.shields.io/static/v1?label=Slides&message=Google%20Slides&color=tomato" alt="Google Slides"/>
  </a>
  <br><br>
  <h4>Ejecuta el código:</h4>
  <a href="https://colab.research.google.com/github/GabrielMissael/cdecmx/blob/main/C%20-%20Intro%20a%20Pandas.ipynb" target="_blank">
    <img width="30%" src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
  </a>
</center>

<!-- Buttons -->
<br>
<div class="buttons has-addons is-centered">
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-4B/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-1C/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-2C/">Siguiente ▶︎</a>
</div>

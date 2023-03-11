---
title: "Bloque 2:"
subtitle: >
   - Revisando los datos. <br>
   - Selección de datos por etiqueta. <br>
   - Selección de datos por posición.
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-2C
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

# Introducción a Pandas - Bloque 2

<br>
<center>
  <img width="50%" src="https://pandas.pydata.org/docs/_static/pandas.svg">
</center>
<br>

En esta sección aprenderás lo básico sobre Pandas, al menos a un nivel conceptual. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Revisando los datos.
- Selección de datos por etiqueta.
- Selección de datos por posición.

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://www.youtube.com/embed/ueYwoVkNg0c" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## Revisando los datos.
 
Para visualizar los datos de un DataFrame, tenemos dos opciones:
 
```python
# Mostramos las primeras 7 filas.
df.head(n = 7)
 
# Mostramos las últimas 4 filas.
df.tail(n = 4)
```

Si queremos ver un DataFrame completo, lo ponemos solo en una celda.
 
```python
# Para ver todo el DataFrame
df
```

Si el DataFrame es muy grande, no se podrá visualizar completo.

Además de consultar partes del DataFrame, también podemos consultar las etiquetas en las **filas** y las **columnas**, así como todos los **valores** del DataFrame.
 
```python
columnas = df.columns  # Obtenemos columnas
indice = df.index  # Obtenemos filas
valores = df.values  # Obtenemos valores
```

Finalmente, cuando tenemos un conjunto de datos, nos será útil hacer un análisis inicial (exploratorio) de los datos. Si consideramos que en las columnas tenemos **variables** y en las filas distintos registros de estas, podemos obtener valores de interés con: 
 
```python
# Describimos en general el DataFrame
df.describe()
```

Obtenemos valores de interés de las variables, como el valor máximo, valor mínimo, media, etc. Pero, ¿qué pasa si tenemos las variables en las filas?. Podemos **trasponer** el DataFrame, de manera similar a lo que se hizo en el módulo de NumPy:
 
```python
# Trasponemos un dataframe y guardamos el resultado
df_traspuesto = df.T
```

## Selección de datos por etiqueta.
 
Podemos seleccionar una o varias **columnas** específicas de un DataFrame utilizando las etiquetas. Se crea un nuevo **DataFrame** con las columnas especificadas. 
 
<center>
    <img width="60%" src="https://pandas.pydata.org/docs/_images/03_subset_columns.svg">
</center>
 
De manera similar, podemos seleccionar **filas** utilizando el índice. Podemos seleccionar una o varias filas y se crea también un nuevo **DataFrame**
 
<center>
    <img width="70%" src="https://pandas.pydata.org/docs/_images/03_subset_rows.svg">
</center>
 
Para seleccionar utilizando las **etiquetas** (nombres de filas y columnas) usamos el método **loc()**. Funciona como sigue:
 
```python
# Seleccionamos una sola columna.
serie_columna = df.loc[:, ['Columna1']]
 
# Seleccionamos más de una columna.
df_columnas = df.loc[:, ['Columna1','Columna2']]
 
# Seleccionamos más de una fila.
df_filas = df.loc[['Indice1', 'Indice2'], :]
```

Es importante notar que esta selección no afecta al DataFrame original, y que además lo que no se selecciona se conserva (por ejemplo, al seleccionar una sola columna, el nuevo DataFrame conserva todas las filas).

También puedes seleccionar al mismo tiempo columnas y filas:

<center>
    <img width="70%" src="https://pandas.pydata.org/docs/_images/03_subset_columns_rows.svg">
</center>

Finalmente, puedes obtener una única celda de dos maneras:

```python
dato = df.loc['Fila', 'Columna']
dato = df.at['Fila', 'Columna'] # Lo mismo, pero más rápido
```

## Selección de datos por posición.
 
En la sección anterior, seleccionamos dado a **etiquetas**, esto es, con los nombres de las filas y las columnas. Podemos hacer lo mismo pero está vez con la **posición**. Para esto, en lugar de **loc()** y **at()**, usamos **iloc()** y **iat()**. 
 
```python
# Seleccionamos las primeras 2 columnas.
df_columnas = df.iloc[:, 0:1]
 
# Seleccionamos las últimas 3 filas
df_filas = df.iloc[-3:, :]
 
# Elemento unico
dato = df.iat[0, 0]
```

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vRQNzvUx7qw6JHzbTIcyeGchj8Yvcgt6cEW--nn97_LrH7OtM97z5lIYQl7ETz-YMRcPGPCtVYq0OL5/pub?start=false&loop=false&delayms=3000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-1C/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-2C/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-3C/">Siguiente ▶︎</a>
</div>

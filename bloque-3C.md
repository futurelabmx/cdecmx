---
title: "Bloque 3:"
subtitle: >
- Operaciones básicas: Estadísticos <br>
- Operaciones básicas: Apply <br>
- Unión de datos: Concatenación <br>
- Bonus: Gráficas en Pandas.
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-3C
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

# Introducción a Pandas - Bloque 3

<br>
<center>
  <img width="50%" src="https://pandas.pydata.org/docs/_static/pandas.svg">
</center>
<br>

En esta sección aprenderás lo básico sobre Pandas, al menos a un nivel conceptual. Hemos preparado un video explicativo para ti, donde cubriremos los siguientes temas:

- Operaciones básicas: Estadísticos
- Operaciones básicas: Apply
- Unión de datos: Concatenación
- Bonus: Gráficas en Pandas.

<figure class="image is-16by9">
  <iframe class="has-ratio" src="https://www.youtube.com/embed/xm4jKcZDdxc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

## Operaciones básicas: Estadísticos.
 
Como se ha mencionado anteriormente, en cada columna normalmente se tendrá una **variable**, como nombres, edad, etc. y en cada fila habrá un registro de esa variable. Hay diversos **estadísticos** que podemos calcular para conocer más sobre la variable y como se comporta. Por ejemplo, si suponemos que una variable sigue un comportamiento normal, entonces conocer su media (promedio) $\mu$ y su desviación estándar $\sigma$ nos será de mucha utilidad. Si $\mu = 10$ y $\sigma = 3$, tenemos:
 
<center>
    <img width="40%" src="https://i.imgur.com/aqUvIQK.png">
</center>
 
Si quieres ver como hacer una gráfica como esta con Python, visita este [link](https://gist.github.com/GabrielMissael/6987ffd5e7fd83e2906ae201245d847b#file-normal_dist-py). Ya obtuvimos algunos valores con **.describe()**, y ahora veremos algunas otras funciones útiles.
 
```python
# Obtenemos la media de todas las columnas
promedios = df.mean()
 
# Media de una sola columna usando .loc()
promedio = df.loc[:,'Columna1'].mean()
 
# Podemos usar describe() en solo una sección del df
descripcion = df.iloc[0:15, [2, 4]].describe()
 
# También podemos obtener la desviación estándar
stds = df.std()
 
# Valores mínimos y máximos
maxs = df.max()
mins = df.min()
```

## Operaciones básicas: Apply.
 
En muchas ocasiones, no sólo estaremos interesados en consultar o describir los datos, si no también en **operarlos**. Podemos aplicar funciones a los datos para obtener valores de interés. Para esto, usamos **.apply()**.
 
```python
# Aplicamos la función seno a los datos
df_seno = df.apply(np.sin)
```

## Unión de datos: Concatenación
 
Podemos unir dos DataFrames. Si ambos comparten columnas, entonces será como agregar más filas al final: 
 
<center>
    <img width="70%" src="https://pandas.pydata.org/docs/_images/08_concat_row.svg">
</center>
 
Si se tienen algunas columnas diferentes, el DataFrame final tendrá columnas extra y **valores faltantes** (aunque también puedes elegir eliminar las columnas que no coinciden).
 
Para esto, usamos: 
 
```python
# Unimos dos DataFrames.
df_nuevo = pd.concat([df1, df2])
```

## Bonus: Gráficas en pandas.

Podemos gráficar fácilmente los datos en un DataFrame:

```python
# Gráfica de linea
df.plot(x = 'Columna1', y = 'Columna2')

# Gráfica de puntos
df.plot.scatter(x = 'Columna1', y = 'Columna2')
```

<center>
  <br>
  <h4>Revisa los slides:</h4>
  <a href="https://docs.google.com/presentation/d/e/2PACX-1vS_ZTnjhiRdh7usbTgdtbY5KitXpktoCIwLv0GTXfr3iYtwYdEurOmbJxhAR_bWR9xx-RwTcrZaysGY/pub?start=false&loop=false&delayms=60000" target="_blank">
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
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-2C/">◀︎ Anterior</a>
  <a class="button is-warning" href="{{ site.baseurl }}/test-3C/">📝 Realizar prueba del módulo</a>
  <a class="button is-outlined" href="{{ site.baseurl }}/bloque-1D/">Siguiente ▶︎</a>
</div>

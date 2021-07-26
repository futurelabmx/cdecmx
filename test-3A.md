---
title: "Prueba de conocimientos:"
subtitle: >
  - Introducción a Python
layout: page
show_sidebar: false
hide_footer: false
menubar: site_menu
tabs: test-3A
---

# Prueba del módulo A

<br>
<center>
    <img width="50%" src="https://www.python.org/static/community_logos/python-logo-generic.svg">
</center>

Lee atentamente los comentarios contenidos en el siguiente bloque de código. Allí encontrarás las indicaciones paso a paso de lo que deberás ir realizando. 

> Nuestra sugerencia es que copies y pegues las indicaciones en una nueva celda de tu cuaderno Colab para que puedas resolver el ejercicio y comprobarlo antes de ejecutar el código dentro de este bloque.

<div data-datacamp-exercise data-lang="python">
	<code data-type="pre-exercise-code">
		# This will get executed each time the exercise gets initialized
		
	</code>
	<code data-type="sample-code">
		# Crea una variable entera llamada
		# edad y asigna a ella el valor de
		# 21


		# Imprime el valor de la variable edad


		# Verifica si la edad es mayor de 18
		# e imprime un mensaje en pantalla
		# con el texto "Eres mayor de edad."
		# En caso contrario, imprime
		# un mensaje en pantalla con el
		# texto "Eres menor de edad."





		# Escribe un ciclo for utilizando
		# la función range para imprimir
		# una pirámide de *, de 1 hasta
		# 10; la salida debe verse así:
		# *
		# **
		# *** (y así hasta 10 *'s)



		# Crea una lista con los meses
		# del año, comenzando en mayúsculas


		# Crea una función que se llame
		# meses_e que reciba como parámetro
		# la lista meses y que devuelva
		# la lista  de los meses que
		# terminan en "e"
		def meses_e(meses):
			# Crea una lista vacía a la que
			# se le añadirán los meses que
			# terminan en "e"
			meses_con_e = []

			# Tu código va aquí
			
			return meses_con_e
		
		# Imprime la lista de los meses
		# que terminan en "e" usando la
		# función meses_e
		

		# Finalmente, crea un diccionario
		# llamado clubera, que contenga los
		# pares clave-valor siguientes:
		# "nombre" - "Cris"
		# "edad" - "27"
		# "sede" - "Guanajuato"
		# "area" - "bio"


		# E imprime el valor de la sede
		# usando corchetes
	</code>
	
  	<code data-type="solution">
		# Crea una variable entera llamada
		# edad y asigna a ella el valor de
		# 21
		edad = 21

		# Imprime el valor de la variable edad
		print(edad)

		# Verifica si la edad es mayor de 18
		# e imprime un mensaje en pantalla
		# con el texto "Eres mayor de edad."
		# En caso contrario, imprime
		# un mensaje en pantalla con el
		# texto "Eres menor de edad."
		if int(edad) >= 18:
			print("Eres mayor de edad.")
		else:
			print("Eres menor de edad.")
		
		# Escribe un ciclo for utilizando
		# la función range para imprimir
		# una pirámide de *, de 1 hasta
		# 10; la salida debe verse así:
		# *
		# **
		# *** (y así hasta 10 *'s)
		for i in range(1, 11):
			print("*" * i)
		
		# Crea una lista con los meses
		# del año, comenzando en mayúsculas
		meses = [
			"Enero",
			"Febrero",
			"Marzo",
			"Abril",
			"Mayo",
			"Junio",
			"Julio",
			"Agosto",
			"Septiembre",
			"Octubre",
			"Noviembre",
			"Diciembre"
		]

		# Crea una función que se llame
		# meses_e que reciba como parámetro
		# la lista meses y que devuelva
		# la lista  de los meses que
		# terminan en "e"
		def meses_e(meses):
			# Crea una lista vacía a la que
			# se le añadirán los meses que
			# terminan en "e"
			meses_con_e = []

			# Recorre la lista meses
			for mes in meses:
				if mes[-1] == "e":
					meses_con_e.append(mes)
			
			return meses_con_e
		
		# Imprime la lista de los meses
		# que terminan en "e" usando la
		# función meses_e
		print(meses_e(meses))

		# Finalmente, crea un diccionario
		# llamado clubera, que contenga los
		# pares clave-valor siguientes:
		# "nombre" - "Cris"
		# "edad" - "27"
		# "sede" - "Guanajuato"
		# "area" - "bio"
		clubera = {
			"nombre": "Cris",
			"edad": "27",
			"sede": "Guanajuato",
			"area": "bio"
		}

		# E imprime el valor de la sede
		# usando corchetes
		print(clubera["sede"])
	</code>
	
  	<code data-type="sct">
		test_object("edad")
		test_function("print")
		test_output_contains("21")
		test_output_contains("Eres mayor de edad.")
		test_student_typed("for")
		test_student_typed("range")
		test_object("meses")
		test_function("meses_e")
		test_object("clubera")
		test_output_contains("Guanajuato")
		success_msg("¡Buen trabajo!")
	</code>

	<div data-type="hint">Para la función de meses te recomendamos utilizar un ciclo <code>for</code> y usar indexación con corchetes <code>mes[-1]</code> para verificar la última letra del mes.</div>
</div>

<!-- Buttons -->
<br>
<div class="buttons has-addons is-centered">
  <a class="button is-info is-large" href="{{ site.baseurl }}/bloque-1B/">🚀 Continuar al módulo B</a>
</div>
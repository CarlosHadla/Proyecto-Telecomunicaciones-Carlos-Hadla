# [LAB02-HENRY](https://github.com/CarlosHadla/Proyecto-Telecomunicaciones-Carlos-Hadla#LAB02-HENRY)

#### [**Contexto**](https://github.com/CarlosHadla/Proyecto-Telecomunicaciones-Carlos-Hadla#contexto)

En este escenario, se enfoca en la industria de las telecomunicaciones en Argentina y la necesidad de comprender y analizar su comportamiento a nivel nacional. El rol a desarrollar es el de un Data Analyst que trabaja para una empresa de telecomunicaciones. La empresa se especializa en brindar acceso a Internet, pero también busca comprender el comportamiento de otros servicios de comunicación para mejorar la calidad de sus servicios y ofrecer soluciones personalizadas.

Aca va el kpi original y el propuesto:
--
--
--
--


**Variables en los dataset y relación:**
--
--
--
--


#### [**ETL**](https://github.com/CarlosHadla/Proyecto-Telecomunicaciones-Carlos-Hadla#etl)

En el notebook [ETL](https://github.com/CarlosHadla/Proyecto-Telecomunicaciones-Carlos-Hadla/ETLySeleccionDeDatos.ipynb), se observa la importación de los dataset y se empieza a hacer una limpieza.

**1. Objetivos:**

- Limpeza y corrección de nombres, tipos de dato, datos vacios, etc.  
- Visualizar la naturaleza de los dataset y las relaciones entre estos.
- Seleccionar los datos a usar en el EDA según las relaciones encontradas.

**2. Selección y relaciones:** 

- Se separaron los dataframes en 3 categorias: 'na' (Nación), 'prov' (Provincia) y 'loc' (Localidad)
- Se relacionó los datos según años y trimestres

- Se seleccionaron los datos de 'Nación' y 'Provincia' para realizar el EDA, ya que los dataframes categorizados como 'Localidad' no tienen datos de tiempo
- Se retiro el dataframe 'prov_dis_accesos_todo_vel_bajada', ya que 'prov_dis_accesos_rango_vel_bajada' contiene los mismos datos agrupados en rangos y abarca todos los años (2014-2022)
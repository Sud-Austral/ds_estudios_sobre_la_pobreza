
# Estudios sobre la pobreza

<a href="url"><img src="madre_migrante.jpg" align="left" height="300" ></a>

**La casen del 2020** trae dos particularidades:

1 en vez de ceros, trae NAs, al contrario de todas las demas casen\
2 no tiene campo alfabetismo, que construimos a partir de una regresión lineal en el repositorio:
**ds_estimacion_con_RL_de-analf_2020**\

***

1.1 Existe un programa **pobreza_NM.Rmd**, el cual
identifica un error que se observa en las publicaciones oficiales de pobreza de las Casen 
2006, 2009 y 2011 el que se produce al ser aplicada las Casen originales (debido a la crisis subprime la
cantidad de pobres en vez de aumentar, desciende). Se corrige con una nueva metodologia 

Para ello tuvimos que utilizar las bases de datos:

1. Ingresos MN 2006.sav
2. Ingresos MN 2009.sav
3. Ingresos MN 2011.sav

Éstas tablas dicen "Ingresos" por lo que son parciales y por lo que hubo que construir una clave para unirlas 
con las tradicionales.

Aplicando nuestros análisis con estas bases de datos coincidimos con la data publicada oficial.

El programa más importante que recoge las Casens corregidas y establece porcentajes de pobreza por comuna 
de acuerdo a la nueva metodologia es **pobreza_NM.RMD**

En la carpeta:

porcentaje_de_pobreza_por_comuna_xlsx/

están las frecuencias de no pobres, pobres y pobres extremos y la frecuencia de pobres por comunas 
(la unión de pobres y pobres extremos) para las 7 Casen 2006-2020 (para cada año), una tabla unida
y una tabla interpolada con el porcentaje de pobreza entre los años 2006 y 2020.



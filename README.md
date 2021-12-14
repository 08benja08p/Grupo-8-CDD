# Introducción

### **Indice**

1. [Extracción de datos/Limpieza](https://08benja08p.github.io/Grupo-8-CDD/#extracci%C3%B3n-de-datoslimpieza-de-datos)
2. [Procesamiento y transformación](https://08benja08p.github.io/Grupo-8-CDD/#procesamiento-y-transformaci%C3%B3n)
3. [Analisis exploratorio](https://08benja08p.github.io/Grupo-8-CDD/#analisis-exploratorio)
4. [Aprendizaje supervisado](https://08benja08p.github.io/Grupo-8-CDD/#aprendizaje-supervisado)
5. [Aprendizaje no supervisado](https://08benja08p.github.io/Grupo-8-CDD/#aprendizaje-no-supervisado)
6. [Conclusiones y visualizaciones al cierre](https://08benja08p.github.io/Grupo-8-CDD/#conclusiones-y-visualizaciones-al-cierre)
7. [Sobre nosotros](https://08benja08p.github.io/Grupo-8-CDD/#Sobre-nosotros)

**Título del proyecto**: Influencia de factores sociodemográficos en el número de delitos por comuna.

**Contexto y motivación**: El presente proyecto busca medir proyecciones sobre el aumento o disminución de los niveles de delincuencia por tipo de incidentes considerando todas las comunas de Chile disponibles en la muestra, además se considera factores como índice de pobreza, población, superficie e incluso fase de paso a paso para los años de pandemia

**Objetivo general**: Disponer de una mirada general país y también específica en delitos por comuna, en base a datos de fuentes oficiales para obtener una radiografía de la situación nacional que permita direccionar la toma de decisiones de forma comunal en materia social.

**Audiencia del público**: a la opinión pública (todo público) y organismos tanto públicos como privados para la toma de decisiones sociales relacionadas a la delincuencia.

# Extracción de datos/Limpieza de datos

los datos utlilizados en este proyecto fueron los siguientes:

1. [Delitos registrados por CEAD](http://cead.spd.gov.cl/centro-de-documentacion/?wpdmpro=estadisticas-anuales-delitos-de-mayor-connotacion-social-dmcs-base-censo-2017)

2. [Datos calidad educación](http://datos.mineduc.cl/dashboards/20014/descarga-bases-de-datos-sned/)

3. [Datos pobreza](http://observatorio.ministeriodesarrollosocial.gob.cl/storage/docs/pobreza-comunal/2017/PLANILLA_Estimaciones_comunales_tasa_pobreza_por_ingresos_multidimensional_2017.xlsx)

4. [Información comunas](https://github.com/MinCiencia/Datos-COVID19/blob/master/input/Otros/InformacionComunas.csv)

5. [Datos natalidad](https://github.com/MinCiencia/Datos-COVID19/tree/master/input/RegistroCivil)

6. [Datos mortalidad](https://github.com/MinCiencia/Datos-COVID19/tree/master/input/RegistroCivil)

7. [Datos salud](https://repositoriodeis.minsal.cl/DatosAbiertos/Establecimientos_ChileDEIS_MINSAL%2010-12-2021.xlsx)

# Procesamiento y transformación

La primera etapa del proyecto, luego de recabar los datos a utilizar, fue procesar los datos obtenidos. El objetivo principal de esta etapa consistió en lograr generar un dataset que incluyera toda la información recabada en un solo lugar. Lo anterior constituyó un gran desafío, dada las diferencias de tipeos de nombres que se encontraron en los datasets. Para lograr superar esa barrera, se utilizó una estandarización de nombres que consideraba la extracción de caracteres especiales y normalización a minúsculas, lo cual no fue suficiente. Se requirió de un análisis caso a caso para lograr la constitución del dataset buscado.

IMAGEN DEL DATASET  obtenido


# Analisis exploratorio

Desde la primera etapa del análisis exploratorio, que consistía en la detección de valores outliers, comenzaron a surgir datos de interés. Entre los que vale la pena destacar, se encontró que la cantidad de delitos de mayor connotación social en la comuna de Santiago es la mayor a nivel nacional; lo sorprendente, es que en segundo lugar se encuentra Puente Alto, pero con sólo la mitad del promedio respecto a la comuna de Santiago. Se comprobó que dicha información es consistente. 
También se encontró que la comuna con mayor cantidad de defunciones por año a nivel país es la comuna de Independencia. Análogamente a la situación anterior, la cantidad de defunciones por año en Independencia es prácticamente el doble de las defunciones de la comuna que le sigue, que corresponde a la comuna de Santiago. No se encontró una explicación lógica para lo anterior.
Se realizó un análisis de las distribuciones de las distintas variables según región. De este análisis surgieron algunas conclusiones de relevancia:
•	En cuanto a la superficie en km2 de las comunas, destacan en particular las regiones del extremo norte de Chile y del extremo sur, que presentan las comunas con más superficie en km2 en comparación con el resto de las regiones.

•	En cuanto al porcentaje de pobreza, la región metropolitana posee una concentración en los valores medios e inferiores de esta variable, presentando un panorama bastante más favorable que el resto de las regiones. La región con menos porcentaje de personas en pobreza multidimensional parece ser la región de Magallanes. Las comunas con mayor porcentaje de personas en situación de pobreza multidimensional se encuentran en las región de Arica y Parinacota, región de Tarapacá y región del Biobío, principalmente.

•	En cuanto a la calidad de la educación, en este caso destacan las regiones del norte de Chile y la XIV región de los Ríos, que en comparación con el resto de las regiones presentan niveles notablemente menores de calidad de educación. En el resto de las regiones se observa una distribución más transversal y equitativa de la calidad de educación en las comunas. Destacan por tener varias comunas con alto nivel de calidad de educación las regiones Metropolitana y VI región (O'Higgins).

•	Respecto del promedio de delitos, se puede observar que en comparación a la región metropolitana, el resto de las regiones parece tener una concentración hacia los valores inferiores de esta variable. Además, se puede observar que en la región metropolitana la distribución de los promedios de delitos es transversal: se abarca desde comunas con bajo promedio de delitos hasta comunas que presentan los mayores promedios de delitos a nivel nacional. La región de magallanes es la que presenta menor promedio de delitos anuales. 


•	(grafico de distribución delitos por región)

Cuando se realizó un primer análisis de las relaciones de las distintas variables con la cantidad de delitos de mayor connotación social, no se apreciaron en primera instancia grandes correlaciones, salvo con aquellas variables que se hallan relacionadas con la población (nacimientos, defunciones, y la población en sí). Una relación que cabe destacar es la de la pobreza con los niveles de delincuencia:  se puede observar que las comunas con mayor promedio de delitos anuales se concentran principalmente en los rangos inferiores del porcentaje de pobreza, mientras que en los rangos superiores de porcentaje de pobreza se observa una evidente disminución del promedio de delitos anuales. La situación es bastante similar para el caso de la variable Calidad Educacion, donde se observa una mayor promedio de delitos anuales en aquellas comunas que tienen un mayor nivel de calidad de educación. (grafico porcentaje de pobreza vs delitos)


# Aprendizaje supervisado

Se realizaron 3 modelos de aprendizaje supervisado: Regresión multilineal, Lasso y Ridge. Estos procesos no fueron fructíferos del todo: a pesar de que las métricas de rendimiento no fueron del todo malas, se observó un gran nivel de ruido e imprecisión en las predicciones. Además el modelo Lasso, que fue el que mejor resultados arrojó, solo consideró las variables Población y nacimientos por año, del total de las variables consideradas.
(Gráfico final de las regresiones)



# Aprendizaje no supervisado

Con los datos obtenidos, se realizó un proceso de clustering. Se detectaron 5 clusters relevantes en directa relación a los niveles de delincuencia. En este proceso, también tuvieron gran relevancia las variables de población y nacimientos x año.


# Conclusiones y visualizaciones al cierre

escribir

# Sobre nosotros

<table>
  <tr>
    <td><img src="https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Cristobal.jpg" width="200"></td>
    <td><img src="https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Diego.jpg" width="200"></td>
    <td><img src="https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Benja-Foto.JPG" width="200" ></td>
    <td><img src="https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Larry.jpg" width="200"></td>
  </tr>
  <tr>
    <td>Cristobal Cancino</td>
    <td>Diego Rodríguez</td>
    <td>Benjamín Prieto</td>
    <td>Larry Uribe</td>
  </tr>
  <tr>
    <td>cristobal.cancinob@uc.cl</td>
    <td>drodrguez@uc.cl</td>
    <td>bprietz@uc.cl</td>
    <td>larry@uc.cl</td>
  </tr>
</table>

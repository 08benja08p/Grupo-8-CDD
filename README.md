# Introducion

Nuestro grupo para el proyecto final de Intro a Ciencia de Datos es:

Cristóbal Cancino - cristobal.cancinob@uc.cl

![f1](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Cristobal.jpg "Logo Title Text 1")

Diego Rodríguez - drodrguez@uc.cl

![f2](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Diego.jpg "Logo Title Text 1")

Benjamín Prieto - bprietz@uc.cl

![f3](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Benja-Foto.JPG "Logo Title Text 1")

Larry Uribe - larry@uc.cl

![f3](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto-Larry.jpg "Logo Title Text 1")

**Título del proyecto**: Influencia de los factores sociales y económicos en la proyección de la delincuencia.

**Contexto y motivación**: El presente proyecto busca medir proyecciones sobre el aumento o disminución de los niveles de delincuencia por tipo de incidentes considerando todas las comunas de Chile disponibles en la muestra, además se considera factores como índice de pobreza, población, superficie e incluso fase de paso a paso para los años de pandemia

**Objetivo general**: Disponer de una mirada general país y también específica en delitos por comuna, en base a datos de fuentes oficiales para obtener una radiografía de la situación nacional que permita direccionar la toma de decisiones de forma comunal en materia social.

**Audiencia del público**: a la opinión pública (todo público) y organismos tanto públicos como privados para la toma de decisiones sociales relacionadas a la delincuencia.

### **Nuestro proyecto se dividira en 6 partes**

1. [Extracción de datos/Limpieza](https://08benja08p.github.io/Grupo-8-CDD/#introducion)
2. [Procesamiento y transformación](https://www.google.com)
3. [Analisis exploratorio](https://www.google.com)
4. [Aprendizaje supervisado](https://www.google.com)
5. [Aprendizaje no supervisado](https://www.google.com)
6. [Conclusiones y visualizaciones al cierre](https://www.google.com)

# Extracción de datos/Limpieza de datos

los datos utlilizados en este proyecto fueron los siguientes:

1. [Delitos registrados por CEAD](http://cead.spd.gov.cl/centro-de-documentacion/?wpdmpro=estadisticas-anuales-delitos-de-mayor-connotacion-social-dmcs-base-censo-2017)

2. [Datos calidad educación](https://junar-selfpub-storage.s3.amazonaws.com/0705/50931/140196801712254783814864722173348825596?response-content-disposition=attachment%3B%20filename%3D%2220181218_SNED_2018_2019.csv%22&AWSAccessKeyId=AKIAI652OHJ6H2VI25OA&Expires=1639422218&Signature=gwJYuTTSvlY4%2FR%2Bav1L4kJRkWWI%3D)

3. [Datos pobreza](http://observatorio.ministeriodesarrollosocial.gob.cl/storage/docs/pobreza-comunal/2017/PLANILLA_Estimaciones_comunales_tasa_pobreza_por_ingresos_multidimensional_2017.xlsx)

4. [Información comunas](https://raw.githubusercontent.com/MinCiencia/Datos-COVID19/master/input/Otros/InformacionComunas.csv)

5. [Datos natalidad](https://github.com/MinCiencia/Datos-COVID19/tree/master/input/RegistroCivil)

6. [Datos mortalidad](https://github.com/MinCiencia/Datos-COVID19/tree/master/input/RegistroCivil)

7. [Datos salud](https://repositoriodeis.minsal.cl/DatosAbiertos/Establecimientos_ChileDEIS_MINSAL%2010-12-2021.xlsx)

# Procesamiento y transformación

Dadas variaciones en las convenciones utilizadas para nombrar a las comunas, utilizamos una función para estandarizar tales nombres. Se procedió a aprovechar esto para combinar los datos de todos los datasets ya limpios mencionados previamente, para después comenzar un análisis exploratorio de los datos obtenidos.

# Analisis exploratorio

Durante tal análisis exploratorio, nos encontramos con el curioso dato de que a pesar de que la comuna de Santiago tiene el mayor índice de delitos, la comuna con el mayor registro de defunciones (Fallecimientos), por casi el doble en el período que analizamos, fue la de Independencia.

![f3](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto_1.jpg "Logo Title Text 1")

Este dato sobre Independencia es a pesar de que en Santiago se denuncia una cantidad increíblemente grande de delitos, en comparación a otras regiones. Más del doble que la segunda comuna con más delitos.

![f3](https://github.com/08benja08p/Grupo-8-CDD/raw/main/Fotos/Foto_2.jpg "Logo Title Text 1")

Del dato de Independencia se puede añadir que no se encuentra en el listado de las 10 comunas con más delitos, por lo que es plausible asumir que una gran parte de las defunciones en tal comuna son por motivos no relacionados al crimen.

# Aprendizaje supervisado

escribir

# Aprendizaje no supervisado

escribir

# Conclusiones y visualizaciones al cierre

escribir

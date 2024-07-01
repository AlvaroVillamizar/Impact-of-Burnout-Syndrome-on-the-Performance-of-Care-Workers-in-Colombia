# Estudio estadístico del sindrome de burnout y factores de riesgo psicosociales asociados al control inhibitorio en trabajadores de Colombia

Para este proyecto se empleó un muestreo en trabajadores de Colombia bajo la metodología del efecto bola de nieve, esto debido al difícil acceso a poblaciones de profesionales asistenciales que cuenten con el permiso de la empresa. Los trabajadores de tipo asistencial presentes en este proyecto incluyen policías, docentes y trabajadores de salud, dentro de los trabajadores no asistenciales encontramos operarios y personal de oficina.

Para este proyecto se establecieron una serie de hipótesis las cuales fueron exploradas y resueltas a través del presente análisis, estas hipótesis establecen:

•	¿Existe una relación entre síntomas de burnout en trabajadores asistenciales y no asistenciales con la función ejecutiva de control inhibitorio?

•	¿Existe una relación entre los factores de riesgo psicosociales con los síntomas de burnout en los trabajadores asistenciales y no asistenciales de Colombia?

•	¿Qué dimensión del Síndrome de Burnout presenta mayor prevalencia en la población estudiada?

•	¿Qué dominio de riesgo psicosocial se asocia con mayor intensidad a los síntomas de burnout?

Las variables de estudio se dividen en 3 grupos:
•	**Variables de análisis:** las cuales representan los resultados obtenidos por las técnicas e instrumentos de recolección de datos, estas variables representan síntomas asociados a burnout como: Despersonalización o cinismo, agotamiento emocional y Autorrealización personal.

•	**Control inhibitorio:** las cuales fueron calculadas por medio de pruebas neuropsicológicas, factores de riesgo psicosocial (Liderazgo, control sobre el trabajo, demandas del trabajo, recompensas, factores extralaborales)

•	**variables de control:** edad; individuos de entre 25 a 60 años,  género; Masculino o Femenino, y nivel de formación; básica secundaria, profesional, técnico o tecnólogo

## Metodología
Para establecer soluciones a las hipótesis planteadas, la metodología implementada fue:

1.	**Procesamiento:** Se limpiaron los datos en Excel, por medio de filtros se identificaron entradas con resultados incorrectos y se eliminaron información de identificación de los participantes del experimento.

2.	**Construcción de la base de datos:** Los resultados de las variables de análisis y las pruebas neuropsicológicas estaban en formatos separadas, por lo que se implementó un algoritmo en Microsoft SQL para unificar la información por medio del número de cédula.

3.	**Exploración de los datos:** Para obtener un primer acercamiento sobre la naturaleza de los datos, se implementaron pruebas de normalidad de Shapiro-Wilks para identificar si las muestras siguen una distribución normal con el fin de establecer las pruebas estadísticas correctas.

4.	**Análisis estadístico:** En esta sección se diseño un análisis de correlación para medir la fuerza y dirección de la relación lineal entre las variables de estudio. Posteriormente se clasificaron cada variable en categorías para estudiar la existencia de correlación dentro de subgrupos.

## Exploración de los datos:

Se inició la exploración de los datos implementando gráfico de barras y circulares para observar la distribución de la población de profesionales asistenciales y no asistenciales en la base de datos, los resultados se presentan en la Figura 1. Los resultados apuntaron a que los datos se encontraban desequilibrados, puesto que el grupo de los profesionales asistenciales representa casi el 80% de todos los datos, esto nos indica que hay que es recomendable estratificar los datos para asegurar la inclusión del grupo de los no asistenciales en el análisis.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_13_1.png" width="auto" height="auto">
<figcaption> <strong>Figure 1.</strong>  </figcaption>
</p>
</figure>

Posteriormente se crearon histogramas y gráficas de densidad para identificar diferencias entre los grupos de profesionales en cada una de las variables de estudio, en la Figura 2 se muestran los resultados obtenidos para la variable de despersonalización.

Adicional a las gráficas antes mencionadas, también se incluyeron:  test de normalidad de Shapiro en cada una de las distribuciones para identificar normalidad en alguna de ellas, test de Mann-Whitney para identificar diferencias entre las medias de los grupos y la medida d de cohen para medir el efecto que tiene el tamaño de las muestras en la diferencia de sus medias.

Los resultados de las pruebas de normalidad de Shapiro Wilks arrojaron que ninguna de las muestras seguía una distribución normal. Utilizando el hecho de que ninguna muestra sigue una distribución normal, se empleó la prueba U de Mann-Whitney, los resultados arrojaron que no existían diferencias significativas entre los dos grupos, en términos de sus medias. Finalmente, para la medida d de cohen se encontró una presencia pequeña que explica la diferencia entre las medias de la variable de realización.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/Figura2.png" width="auto" height="auto">
<figcaption> <strong>Figure 2.</strong>  </figcaption>
</p>
</figure>

Por último, se crearon un diagrama de caja y bigotes para comparar la distribución de las variables asociadas al síndrome de burnout y los tipos de profesionales. Los resultados se pueden observar en la Figura 3. Los resultados no mostraron diferencias significativas dentro de las medidas de tendencia central y de dispersión, tal como las pruebas Mann-Whitney y d de cohen inferían, se observa que el grupo de profesionales no asistenciales presenta mayor prevalencia de síntomas (promedio 5.764) que el grupo de los profesionales asistenciales (promedio 5.561), sin embargo, observando la diferencia entre ellas tomando, la desviación estándar como referente, se observa que dicha diferencia es despreciable.  


<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_18_0.png" width="auto" height="auto">
<figcaption> <strong>Figure 3.</strong>  </figcaption>
</p>
</figure>

### Exploración por categorías

Para la exploración de los datos por categorías se utilizó una clasificaron de las variables asociadas al burnout de acuerdo con el riesgo de los síntomas, los puntos de corte utilizados para dicha clasificación se resumen en la siguiente tabla

<table>

| Medida                       | Bajo Riesgo | Medio Riesgo | Alto Riesgo |
|------------------------------|-------------|--------------|-------------|
| Agotamiento emocional        | 0 - 18      | 19 - 26      | 27 - 54     |
| Despersonalización o Cinismo | 0 - 5       | 6 - 9        | 10 - 30     |
| Autorrealización personal    | 40 - 48     | 34 - 39      | 0 - 30      |

<caption>Table 1</caption>
</table>


En ella cada variable se divide por Bajo riesgo o síntomas leves, Medio riesgo o síntomas moderados y Alto riesgo o síntomas graves. De acuerdo con esta clasificación se emplearon nuevamente gráficas descriptivas para estudiar el comportamiento de cada grupo.

Los resultados obtenidos para la variable de despersonalización se observan en la Figura 4. Dentro de la categoría leve del componente de despersonalización, la prueba de Mann-Whitney no arrojó diferencias significativas entre los grupos y la medida d de cohen obtenida fue de: -0.32, lo cual indica que el grupo de profesionales asistenciales tuvo mayor prevalencia de estos síntomas (promedio 1.557) con respecto a los profesionales no asistenciales (promedio 1), sin embargo, estos efectos fueron pequeños. Resultados similares se obtuvieron para las categorías moderadas y graves, en éste último se encontró que el grupo de profesionales no asistenciales tuvo mayor prevalencia de estos síntomas (promedio 15.438) con respecto a los profesionales asistenciales (promedio 13.56), sin embargo, estos efectos fueron pequeños.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/Figura4.png" width="auto" height="auto">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/Figura4_2.png" width="auto" height="auto">
</p>
</figure>

## Análisis estadístico

Para determinar si el impacto de los síntomas de Burnout difiere entre profesionales asistenciales y no asistenciales, se realizó un análisis de correlación. Primero se calcularon la correlación de los datos ver Figura 5, para luego dividirlos entre grupos de acuerdo con el tipo de profesional (asistencial y no asistencial), con el fin de recalcular sus correlaciones y observar si existe un cambio que permita encontrar una prevalencia de los síntomas.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/Figura5.png" width="auto" height="auto">
<figcaption> <strong>Figura 5.</strong>  </figcaption>
</p>
</figure>

De la gráfica anterior se puede observar que los componentes de burnout (despersonalización, agotamiento y realización) presentan correlaciones despreciables para predecir el control inhibitorio, además a diferencia del agotamiento y despersonalización, no existen correlaciones entre los componentes, por lo que se necesita investigar por categorías antes de descartar una correlación. En términos generales, las variables inhibición Ac e inhibición (Tmp_RTA) no presentan correlación alguna con las demás variables de estudio.

### Categorías dentro de los componentes del Síndrome de Burnout

Para esa subsección se estudiaron las correlaciones entre el control inhibitorio, las categorías del burnout y el tipo de profesional. Como referencia, a continuación, se muestran los coeficientes de correlación entre los grupos de profesionales, control inhibitorio y las variables de burnout.


<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_64_0.png" width="auto" height="auto">
</p>
</figure>

Se observa que los resultados del test U de Mann-Whitney no encontró diferencias entre los tipos de profesionales, dentro de las categorías de la variable 'inhibición_Ac'. En el análisis de correlación se encontró un aumento en la relación lineal entre síntomas de agotamiento y número de aciertos en profesionales no asistenciales, en comparación con la correlación general encontrada. en la gráfica de dispersión se observa como la recta que se ajusta a los datos tuvo una correlación de 0.07 y luego el coeficiente de correlación aumentó a 0.13. Ver Figura 6


<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_66_1.png" width="auto" height="auto">
<figcaption> <strong>Figura 6.</strong> </figcaption>
</p>
</figure>

El mismo comportamiento se observa para los síntomas de realización, pasando de un coeficiente de correlación de 0.03 a 0.1.

### Impacto del cinismo en el control inhibitorio

Para este análisis se muestran los coeficientes de correlación entre el control inhibitorio, los componentes del burnout y las categorías de despersonalización establecidas en la Tabla 1.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_75_0.png" width="auto" height="auto">
</p>
</figure>

En el análisis de correlación se encontró un aumento en la relación lineal entre síntomas de Despersonalización y Tiempo de Respuesta dentro de las categorías de síntomas Moderados y Graves, en comparación con la correlación general encontrada. En la gráfica de dispersión se observa como la recta que se ajusta a los datos tuvo una correlación de 0.04 y luego el coeficiente
de correlación aumentó a 0.1 y 0.17, respectivamente. Ver Figura 7


<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_77_1.png" width="auto" height="auto">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_77_2.png" width="auto" height="auto">
<figcaption> <strong>Figura 7.</strong> Content summary for the HR-Employee dataset. </figcaption>
</p>
</figure>

Adicionalmente, se encontró un aumento en la relación lineal entre síntomas de Despersonalización y Número de Aciertos dentro de las categorías de síntomas Graves, pasando de un coeficiente de correlación nulo a 0.11.

### Impacto del Liderazgo en el desarrollo del Síndrome de burnout

Para esta subsección se buscó establecer la relación del Liderazgo (Componente del control inhibitorio) y los componentes del burnout, para ello se presenta los coeficientes de correlación del liderazgo con cada una de las variables de estudio. Posteriormente se llevó a cabo la misma metodología que en la sección anterior.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_93_0.png" width="auto" height="auto">
</p>
</figure>

En el análisis de correlación se encontró que: dentro de la categoría de síntomas de agotamiento leves, la correlación entre la agotamiento y Liderazgo total (Lid_total) aumentó, lo que indica que a medida que el agotamiento aumenta, el factor de liderazgo disminuye a un ritmo más desacelerado. En la Figura 8 de dispersión se observa como la recta que mejor se ajusta a los datos tuvo una correlación de -0.24 y luego aumentó a -0.07. Dentro de la categoría de síntomas de agotamiento graves, el comportamiento fue, al contrario, en la gráfica de dispersión el coeficiente de correlación bajó de -0.24 a -0.34, lo cual indica que a medida que los síntomas de agotamiento aumentan, el factor de liderazgo disminuye a un ritmo más acelerado, sin embargo, únicamente el 8.8% de los datos se encontraron dentro de la categoría de síntomas graves, por lo que, debido a la falta de datos, este coeficiente no es preciso.

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_103_1.png" width="auto" height="auto">
<figcaption> <strong>Figura 8.</strong></figcaption>
</p>
</figure>

## correlación de todas las variables del estudio

<figure class="image">
<p align="center">
<img src="https://github.com/AlvaroVillamizar/Impact-of-Burnout-Syndrome-on-the-Performance-of-Care-Workers-in-Colombia/blob/main/Images/output_57_1.png" width="auto" height="auto">
</p>
</figure>

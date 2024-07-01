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

### Metodología
Para establecer soluciones a las hipótesis planteadas, la metodología implementada fue:

1.	**Procesamiento:** Se limpiaron los datos en Excel, por medio de filtros se identificaron entradas con resultados incorrectos y se eliminaron información de identificación de los participantes del experimento.

2.	**Construcción de la base de datos:** Los resultados de las variables de análisis y las pruebas neuropsicológicas estaban en formatos separadas, por lo que se implementó un algoritmo en Microsoft SQL para unificar la información por medio del número de cédula.

3.	**Exploración de los datos:** Para obtener un primer acercamiento sobre la naturaleza de los datos, se implementaron pruebas de normalidad de Shapiro-Wilks para identificar si las muestras siguen una distribución normal con el fin de establecer las pruebas estadísticas correctas.

4.	**Análisis estadístico:** En esta sección se diseño un análisis de correlación para medir la fuerza y dirección de la relación lineal entre las variables de estudio. Posteriormente se clasificaron cada variable en categorías para estudiar la existencia de correlación dentro de subgrupos.

### Exploración de los datos:

Se inició la exploración de los datos implementando gráfico de barras y circulares para observar la distribución de la población de profesionales asistenciales y no asistenciales en la base de datos, los resultados se presentan en la Figura 1. Los resultados apuntaron a que los datos se encontraban desequilibrados, puesto que el grupo de los profesionales asistenciales representa casi el 80% de todos los datos, esto nos indica que hay que es recomendable estratificar los datos para asegurar la inclusión del grupo de los no asistenciales en el análisis.

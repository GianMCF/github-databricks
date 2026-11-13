# Github Databricks - Gianmarco Castillo Flores

# Predicciones futuras del comportamiento de las solicitudes

A partir de los resultados obtenidos mediante las consultas SQL y el
análisis exploratorio del conjunto de datos
`consultas_denuncias_silver`, se plantean las siguientes predicciones
sobre el comportamiento futuro de las solicitudes relacionadas con
consultas y denuncias en salud.

Estas predicciones son **proyecciones cualitativas basadas en los
patrones observados**. No representan resultados de un modelo predictivo
ni estimaciones estadísticas exactas. Además, el periodo analizado
comprende los primeros meses de 2026 y el registro de abril podría
encontrarse incompleto, por lo que las tendencias deberán validarse con
información de periodos posteriores.

## 1. Evolución futura de las solicitudes según el tipo y el mes de registro

### Evidencia observada

El análisis por tipo de solicitud identificó un total de **45 217
registros**:

-   **Consulta:** 22 737 solicitudes (50,3 %).
-   **Denuncia:** 22 466 solicitudes (49,7 %).
-   **Intervención de oficio:** 14 solicitudes (0,03 %).

En el análisis mensual, marzo de 2026 presentó el mayor volumen, con
**16 195 solicitudes (35,8 %)**, seguido de febrero con 12 422 (27,5 %),
enero con 11 102 (24,6 %) y abril con 5 498 (12,2 %).

### Predicción

Si se mantiene el comportamiento observado, es probable que las
consultas y las denuncias continúen concentrando la mayor parte de las
solicitudes registradas. Debido a que ambas categorías presentan
proporciones muy similares, no se observa una diferencia suficientemente
amplia como para afirmar que una de ellas dominará de manera sostenida.

Asimismo, marzo podría representar un periodo de mayor demanda; sin
embargo, se requiere analizar más meses y verificar que abril cuente con
información completa antes de concluir que existe un patrón estacional o
una tendencia de crecimiento.

### Utilidad para STASYS

El dashboard podría incorporar una comparación mensual por tipo de
solicitud y una visualización de tendencias que permita identificar
incrementos, disminuciones y cambios en la composición de las
solicitudes. Esto facilitaría la planificación del seguimiento y la
identificación temprana de periodos con mayor volumen de casos.

## 2. Concentración futura de solicitudes por institución y naturaleza institucional

### Evidencia observada

El análisis de las diez instituciones con mayor cantidad de solicitudes
identificó **14 998 registros**, equivalentes al **33,2 % del total**.
Entre ellas destaca el Seguro Social de Salud (IAFAS), con 4 180
solicitudes. También aparecen establecimientos como el Hospital Nacional
Cayetano Heredia, el Hospital Nacional Arzobispo Loayza y el Hospital
Nacional Edgardo Rebagliati Martins.

Por naturaleza institucional, las categorías con mayor volumen fueron:

-   **Gobierno Regional:** 17 039 solicitudes (37,68 %).
-   **MINSA:** 16 401 solicitudes (36,27 %).
-   **ESSALUD:** 4 584 solicitudes (10,14 %).
-   **ESSALUD (Pública):** 4 180 solicitudes (9,24 %).

En conjunto, las cuatro categorías representan aproximadamente el **93,3
%** de las solicitudes analizadas. También se observa que algunas
categorías agrupan solicitudes de numerosas instituciones, mientras que
ESSALUD (Pública) concentra sus registros en una sola institución.

### Predicción

Es posible que las instituciones y categorías que actualmente concentran
más solicitudes continúen representando una parte importante de la carga
de atención en los siguientes periodos. En particular, las entidades
pertenecientes al Gobierno Regional y al MINSA podrían seguir destacando
por su volumen agregado.

No obstante, un mayor número de solicitudes no demuestra por sí solo un
peor desempeño institucional ni permite determinar la causa de los
casos. Para realizar una evaluación más completa sería necesario
relacionar el volumen con otros indicadores, como el tiempo de atención,
el estado de las solicitudes, su categoría y la cantidad de usuarios
atendidos.

### Utilidad para STASYS

STASYS podría fortalecer el seguimiento institucional mediante rankings,
comparaciones por naturaleza y tipo de institución, y consultas sobre la
evolución de los casos. También sería conveniente incorporar indicadores
de tiempo de atención y estado para distinguir entre concentración de
solicitudes y posibles necesidades de seguimiento.

## 3. Comportamiento futuro de las solicitudes según edad y género de los solicitantes

### Evidencia observada

El análisis propuesto considera la distribución de solicitudes según
grupos de edad y género del solicitante. Para evitar resultados
distorsionados, se contempla validar las edades y considerar como
registros no válidos aquellos valores nulos, negativos o superiores a
120 años. Las edades válidas se agrupan en los siguientes rangos:

-   0 a 17 años.
-   18 a 29 años.
-   30 a 39 años.
-   40 a 49 años.
-   50 a 59 años.
-   60 a 69 años.
-   70 años a más.
-   Sin edad registrada.

La interpretación de esta dimensión debe realizarse a partir de los
resultados efectivos de la consulta, considerando también los registros
sin información de edad o género.

### Predicción

Una vez identificados los grupos de edad y género con mayor cantidad de
solicitudes, será posible observar si esa distribución se mantiene en
periodos posteriores o si aparecen cambios en la participación de
determinados grupos.

Por el momento, sin los resultados cuantitativos de esta consulta, no
corresponde afirmar qué grupo etario o género tendrá una mayor demanda
futura. La predicción deberá actualizarse cuando se disponga de los
conteos y porcentajes correspondientes y se comparen con nuevos periodos
de registro.

### Utilidad para STASYS

El dashboard podría presentar la distribución de solicitudes por grupo
de edad y género, además de permitir filtros por periodo, tipo de
solicitud e institución. Esta información ayudaría a reconocer los
grupos que generan mayor cantidad de registros y a orientar análisis
posteriores, siempre considerando la calidad y disponibilidad de los
datos.

## Consideraciones y limitaciones

-   Las predicciones presentadas son cualitativas y se derivan de
    patrones descriptivos del periodo analizado.
-   La información disponible corresponde a los primeros meses de 2026;
    por ello, no es suficiente para establecer patrones estacionales
    anuales.
-   El menor volumen observado en abril debe interpretarse con cautela,
    ya que el periodo podría no estar completo.
-   La cantidad de solicitudes por institución no constituye, por sí
    sola, una medida de calidad o desempeño institucional.
-   La predicción demográfica requiere incorporar los resultados
    efectivos del análisis por edad y género.
-   Para desarrollar pronósticos cuantitativos sería necesario contar
    con una serie histórica más extensa, validar la integridad de las
    fechas y aplicar modelos de series temporales u otras técnicas
    predictivas, evaluando su desempeño con datos de prueba.

## Conclusión

Los resultados exploratorios permiten identificar que las consultas y
denuncias concentran prácticamente la totalidad de las solicitudes, que
marzo presenta el mayor volumen dentro del periodo observado y que una
proporción importante de los registros se concentra en determinadas
naturalezas e instituciones. Estos hallazgos permiten formular hipótesis
sobre el comportamiento futuro y definir qué indicadores conviene
monitorear.

La incorporación de estas dimensiones en STASYS facilitaría el
seguimiento de las solicitudes y la identificación de variaciones
relevantes. Sin embargo, las proyecciones deberán actualizarse conforme
se incorporen nuevos datos y se validen los resultados, evitando
interpretar las tendencias descriptivas como pronósticos estadísticos
definitivos.

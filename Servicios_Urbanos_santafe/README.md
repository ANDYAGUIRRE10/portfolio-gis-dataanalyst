# Servicios urbanos - Santa Fe

## Descripción del proyecto

Proyecto en desarrollo orientado al análisis espacial y estadístico de la distribución de servicios urbanos en la ciudad de Santa Fe, Argentina.

El proyecto busca integrar herramientas de programación, análisis de datos y Sistemas de Información Geográfica (GIS) para estudiar la distribución
territorial de distintos servicios y caracterizar su presencia en las vecinales de la ciudad.

A partir de datos georreferenciados, se desarrollará un flujo de trabajo reproducible en Python que permita procesar información espacial, calcular
indicadores, realizar análisis estadísticos y generar cartografía temática.

## Objetivos

- Organizar y preparar datos geoespaciales para su análisis.
- Evaluar la calidad y consistencia de los datos de entrada.
- Analizar la distribución espacial de los servicios urbanos.
- Calcular estadísticas e indicadores por vecinal.
- Explorar diferencias territoriales en la cantidad, densidad y diversidad  de los servicios registrados.
- Automatizar la generación de tablas, gráficos y mapas temáticos.
- Integrar herramientas de Python con flujos de trabajo GIS.
- Documentar un procedimiento reproducible que pueda aplicarse a otros conjuntos de datos territoriales.

## Datos y fuentes de información

El proyecto parte de un conjunto de capas vectoriales en formato Shapefile (.shp), correspondientes a servicios urbanos y límites de las vecinales
de la ciudad de Santa Fe.

Las categorías contempladas incluyen:

- Centros de atención médica.
- Clubes.
- Estaciones de seguridad policial.
- Áreas verdes.
- Espacios religiosos.
- Centros de recolección de residuos.
- Límites de las vecinales.

La preparación del conjunto de datos implicó tareas de recopilación de fuentes de información, revisión de registros y verificación de ubicaciones
mediante herramientas de consulta geográfica, incluyendo Google Maps y Street View.

Estas tareas buscan mejorar la consistencia de la información espacial y respaldar la identificación de los elementos representados.

Las fuentes originales, los criterios de selección y las limitaciones de los datos se documentarán a medida que avance el proyecto.

## Metodología prevista

El desarrollo se organizará en las siguientes etapas:

### 1. Exploración y control de calidad

- Inventario de las capas disponibles.
- Revisión de sistemas de coordenadas y tipos de geometría.
- Identificación de geometrías inválidas o vacías.
- Detección de registros duplicados y valores faltantes.
- Verificación de la correspondencia espacial entre los servicios y el   área de estudio.

### 2. Procesamiento y análisis espacial

- Lectura y procesamiento de archivos vectoriales.
- Asignación espacial de los servicios a las vecinales.
- Conteo de registros por categoría y unidad territorial.
- Cálculo de superficies y densidades.
- Generación de tablas consolidadas para el análisis.

### 3. Análisis estadístico

- Estadísticas descriptivas de los servicios registrados.
- Comparación entre vecinales.
- Elaboración de rankings territoriales.
- Análisis de la distribución y variabilidad de los indicadores.
- Exploración de la diversidad de categorías de servicios.

### 4. Visualización y cartografía

- Generación automatizada de mapas temáticos.
- Elaboración de mapas coropléticos por vecinal.
- Creación de gráficos estadísticos.
- Exportación de tablas y capas geográficas procesadas.
- Exploración de alternativas de cartografía interactiva.

### 5. Documentación y reproducibilidad

- Organización del código en módulos reutilizables.
- Documentación del entorno de trabajo.
- Registro de los procedimientos de procesamiento y análisis.
- Publicación de resultados seleccionados.

## Tecnologías y herramientas

El proyecto contempla el uso de las siguientes tecnologías:

| Tecnología | Aplicación |
|---|---|
| Python | Procesamiento y automatización del análisis. |
| Pandas | Limpieza, transformación y análisis de tablas. |
| GeoPandas | Lectura, procesamiento y análisis de datos geoespaciales. |
| Shapely | Operaciones y validaciones geométricas. |
| PyProj | Transformación y manejo de sistemas de coordenadas. |
| NumPy | Operaciones y cálculos numéricos. |
| Matplotlib | Generación de gráficos y cartografía estática. |
| Seaborn | Visualización estadística complementaria. |
| Folium | Exploración de cartografía interactiva. |
| Jupyter Notebook | Exploración y documentación del análisis. |
| Miniconda | Gestión del entorno de Python y sus dependencias. |
| Visual Studio Code | Desarrollo y organización del código. |
| Git y GitHub | Control de versiones y documentación del proyecto. |
| QGIS | Visualización, validación y revisión cartográfica de los resultados. |

Las tecnologías se incorporarán progresivamente según las necesidades
de cada etapa del proyecto.

## Estado del proyecto

**En desarrollo.**

Actualmente, se dispone de capas vectoriales georreferenciadas de servicios urbanos y vecinales de la ciudad de Santa Fe. También se han realizado
tareas de recopilación y verificación de información geográfica.

Las siguientes etapas estarán orientadas a la preparación de los datos en Python, el análisis espacial y estadístico, y la automatización de la producción cartográfica.

## Alcance y limitaciones

El análisis se centrará inicialmente en la información disponible y en la distribución espacial de los servicios registrados.

La cantidad de registros no representa necesariamente la capacidad, calidad, suficiencia o accesibilidad de cada servicio.

La incorporación de variables adicionales, como población, distancias, tiempos de desplazamiento o capacidad de atención, permitiría ampliar el alcance del análisis en futuras etapas.

## Propósito

Este proyecto forma parte de un proceso de aprendizaje y desarrollo profesional orientado a fortalecer competencias en análisis de datos,programación aplicada a GIS, estadística descriptiva y cartografía
automatizada.

Busca integrar herramientas de Python con conocimientos de Sistemas
de Información Geográfica para desarrollar procedimientos reproducibles
de análisis territorial.

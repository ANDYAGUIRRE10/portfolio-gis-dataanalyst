# Análisis de Islas de Calor Urbanas — Santa Fe, Argentina

**GIS & Data Analytics | Teledetección | Python**

## Descripción del proyecto

Este proyecto busca analizar la distribución espacial de la temperatura superficial terrestre (*Land Surface Temperature*, LST) y la vegetación en el área urbana de Santa Fe, Argentina, mediante imágenes satelitales gratuitas y herramientas geoespaciales de código abierto.

El análisis se centrará en explorar la relación entre la temperatura superficial y la cobertura vegetal, integrando técnicas de teledetección, procesamiento de datos raster, análisis exploratorio de datos y cartografía temática.

**Estado: proyecto en desarrollo.**

## Objetivos

- Obtener y procesar imágenes satelitales del área de estudio.
- Estimar la temperatura superficial terrestre (LST) a partir de productos Landsat 8 y 9.
- Calcular el Índice de Vegetación de Diferencia Normalizada (NDVI).
- Explorar la relación espacial entre la temperatura superficial y la vegetación.
- Generar estadísticas descriptivas, tablas y visualizaciones mediante Python.
- Elaborar cartografías temáticas y comunicar los resultados mediante productos GIS.

## Fuentes de datos

- **Landsat 8 y Landsat 9 — Collection 2 Level-2:** productos de temperatura superficial y reflectancia superficial.
- **USGS EarthExplorer:** búsqueda y descarga de imágenes satelitales.
- **Datos geográficos complementarios:** límites urbanos y otras capas de referencia, según su disponibilidad y adecuación al análisis.

La selección de imágenes tendrá en cuenta las fechas de adquisición, la nubosidad, la cobertura espacial y los indicadores de calidad de los datos.

## Tecnologías y herramientas

| Tecnología | Aplicación |
|---|---|
| Python | Procesamiento geoespacial y automatización del análisis |
| Rasterio | Lectura y procesamiento de datos raster |
| NumPy | Cálculos numéricos y operaciones sobre píxeles |
| Pandas | Gestión de tablas y análisis estadístico |
| GeoPandas | Procesamiento vectorial y análisis espacial |
| Matplotlib | Gráficos estadísticos y visualizaciones |
| QGIS | Elaboración de cartografía temática |
| Git y GitHub | Control de versiones y documentación del proyecto |

## Metodología de trabajo

El flujo de trabajo previsto comprende las siguientes etapas:

1. **Obtención de datos:** descarga de escenas Landsat adecuadas y de información geográfica complementaria.
2. **Control de calidad:** revisión de metadatos, máscaras de nubes, píxeles válidos y cobertura espacial.
3. **Procesamiento raster:** aplicación de factores de escala y máscaras de calidad a las bandas satelitales.
4. **Cálculo de indicadores:** obtención de la temperatura superficial en grados Celsius y cálculo del NDVI a partir de la reflectancia superficial.
5. **Análisis exploratorio de datos:** cálculo de estadísticas descriptivas, análisis de distribuciones y exploración de la relación entre LST y NDVI.
6. **Producción cartográfica:** elaboración de mapas temáticos mediante QGIS.
7. **Documentación:** publicación de la metodología, los scripts, los resultados seleccionados y las limitaciones del análisis.

## Productos previstos

- Raster y mapa temático de temperatura superficial terrestre.
- Raster y mapa de distribución de la vegetación mediante NDVI.
- Tablas de estadísticas descriptivas en formato CSV.
- Gráficos y visualizaciones estadísticas.
- Flujo de procesamiento reproducible en Python.
- Proyecto QGIS con los productos cartográficos finales.

## Consideraciones analíticas

La temperatura superficial terrestre representa la temperatura radiométrica de la superficie, no la temperatura del aire medida cerca del suelo.

Los datos térmicos de Landsat tienen una resolución espacial nativa más gruesa que la cuadrícula de 30 m en la que se distribuye habitualmente el producto. El remuestreo no genera nuevas observaciones térmicas independientes.

La relación entre NDVI y LST se examinará estadísticamente, sin asumir que una correlación demuestra por sí sola una relación causal.

También se considerarán la presencia de nubes y sombras, las fechas de adquisición, las condiciones estacionales y la delimitación del área de estudio al interpretar los resultados.

## Estado del proyecto

**En desarrollo — obtención de datos y preparación del flujo de trabajo.**

Los análisis, los resultados estadísticos y los mapas finales se incorporarán a medida que avance el proyecto.

Este proyecto forma parte de mi portfolio GIS y Data Analytics y busca aplicar tecnologías geoespaciales y metodologías reproducibles al análisis de problemáticas territoriales y ambientales.

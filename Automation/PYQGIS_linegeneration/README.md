# 🛣️ Automatización GIS vial: generación de líneas transversales con PyQGIS

**Categorías:** GIS · Automatización · Python · QGIS · Infraestructura vial

## 🎯 Objetivo

Automatizar la generación de líneas transversales perpendiculares al eje de una ruta, a partir de una capa de puntos con progresivas, 
para facilitar la determinación del ancho real del camino en el marco de trabajos de inventario vial.

El proceso permite reducir tareas repetitivas de digitalización y establecer una geometría inicial uniforme para su posterior ajuste.

## ⚙️ Metodología

El flujo de trabajo utiliza dos capas vectoriales:

- **Eje de ruta:** geometría lineal de referencia.
- **Puntos con progresivas:** referencias kilométricas distribuidas a lo largo del trazado.

Mediante un script desarrollado con PyQGIS se automatiza la generación de dos líneas perpendiculares de 25 metros por cada punto seleccionado, 
una hacia cada lado del eje vial.

Se consideran referencias cada 1 km, comenzando en la progresiva 0, y se incorpora también el punto de mayor progresiva.

Las líneas generadas constituyen una geometría preliminar que luego se ajusta manualmente según los límites reales del ancho del camino.

## 🤖 Desarrollo asistido por inteligencia artificial

Se utilizó inteligencia artificial como herramienta de asistencia para la generación del código Python.

El trabajo incluyó la lectura y revisión del código propuesto, la ejecución del proceso en QGIS y la comprobación de los resultados geométricos obtenidos. 
La automatización se integró en un flujo de trabajo GIS que combina generación programática, validación espacial y edición manual posterior.

## 📐 Estructura de la capa de salida

El resultado se almacena en formato GeoPackage (GPKG), con los siguientes campos:

| Campo | Tipo | Descripción |
|---|---|---|
| `FID` | Entero | Identificador automático del GeoPackage. |
| `ID` | Texto | Identificador basado en la progresiva de referencia y el número de línea (1 o 2). |
| `LADO` | Texto | Identificación del lado asignado a cada línea. |
| `PROGRESIVA` | Entero | Progresiva de referencia de la capa de puntos. |

## ✏️ Ajuste manual y carga de atributos

Una vez generadas las líneas, se realiza una edición manual mediante las herramientas de **Digitalización avanzada de QGIS**, 
ajustando cada segmento hasta alcanzar los límites reales del ancho del camino.

Posteriormente, se incorporan tres campos para completar el relevamiento:

- **`len`:** longitud calculada de la línea ajustada.
- **`limite`:** tipo de elementos que delimitan el ancho relevado.
- **`obs`:** observaciones sobre situaciones particulares, como la ubicación de un tramo sobre un puente.

Los valores previstos para el campo `limite` son:

| Valor | Delimitación |
|---|---|
| `alam-alam` | Alambrado a alambrado |
| `edif-edif` | Línea de edificación a línea de edificación |
| `edif_alambado` | Línea de edificación a alambrado |
| `alam-edif` | Alambrado a línea de edificación |

Para mantener un criterio uniforme, las mediciones se organizan por lados opuestos del camino, por ejemplo, norte y sur, u oeste y este.

## 🧰 Tecnologías utilizadas

- **QGIS:** visualización, edición y validación de geometrías.
- **PyQGIS:** automatización de operaciones espaciales.
- **Python:** desarrollo y ejecución del script.
- **GeoPackage:** almacenamiento de datos vectoriales.

## 🎥 Demostración

Se presenta una demostración visual del resultado en QGIS, mostrando la generación de líneas transversales (no se muestra el posterior ajuste 
para representar el ancho real del camino).

Por razones de confidencialidad institucional, no se distribuyen el código fuente ni los datos operativos originales.

## 🔒 Confidencialidad

El desarrollo se realizó en el contexto de tareas de infraestructura vial. La publicación se limita a describir la metodología y mostrar resultados autorizados,
sin divulgar información institucional restringida.

## 💡 Competencias aplicadas

- Automatización de procesos geoespaciales.
- Desarrollo asistido por IA y revisión de código.
- Análisis de geometrías lineales y puntos de referencia.
- Validación de resultados en QGIS.
- Integración de procesos automatizados y edición manual.
- Preparación de datos vectoriales para inventarios viales.

---

**Enfoque:** automatización GIS aplicada a inventarios y relevamientos de infraestructura vial.

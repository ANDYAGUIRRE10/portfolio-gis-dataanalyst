### 🎥 Video demostrativo ###

[https://github.com/ANDYAGUIRRE10/portfolio-gis-dataanalyst/blob/main/graphmodel_example.mp4]

## 📌 Contexto ##

Este proyecto surge a partir de la necesidad de georreferenciar grandes volúmenes de datos provenientes de planillas Excel utilizadas en relevamientos de infraestructura vial (alcantarillas, señalización, iluminación, etc.). Cada planilla presentaba formatos distintos, errores de tipeo, columnas con nombres inconsistentes y datos faltantes, lo que hacía imposible una automatización directa sin una etapa previa de criterio humano.

## 🧠 La importancia del criterio humano antes de automatizar ##

Automatizar sin entender los datos es un error común. En este proyecto, el primer paso no fue programar, sino analizar críticamente cada planilla:

- ¿Cómo están escritas las coordenadas? (grados decimales, grados/minutos/segundos, separadores con coma o punto)
- ¿Qué columnas representan realmente la ubicación? (algunas planillas tenían múltiples columnas de coordenadas, otras solo una)
- ¿Qué tipo de objeto se está relevando? (alcantarilla, señal, luminaria, etc.)
- ¿Qué campos son obligatorios y cuáles opcionales a nuestro interés?
- ¿Qué hacer con los errores de tipeo o valores atípicos?

Cada ruta presentaba miles de objetos con estructuras diferentes. Un modelo automático que funcione para una planilla puede fallar en otra si no se ajusta manualmente el criterio de interpretación.

## ⚙️ Proceso realizado ##

- Revisión manual y limpieza de datos: Análisis de la planilla original en Excel, identificación de formatos heterogéneos, corrección de errores y estandarización a un formato CSV único.

- Creación de un modelo gráfico en QGIS que:

Lee el CSV limpio.

Interpreta las columnas de coordenadas según el tipo de dato (x, y).

Genera automáticamente una capa de puntos en formato GeoPackage.

Carga los atributos asociados a cada punto (tipo de objeto, ruta, observaciones, etc.).

- Ejecución y verificación: Corrida del modelo sobre el CSV limpio, generación de la capa de puntos y revisión de la tabla de atributos para asegurar que cada objeto quedó correctamente representado.

## 🎯 Resultado ##

-> Capa de puntos georreferenciados en GeoPackage con miles de objetos de infraestructura vial.

-> Tabla de atributos completa con la información original de la planilla, lista para análisis espacial.

-> Modelo reutilizable que puede adaptarse a nuevas planillas ajustando únicamente los parámetros de entrada según el formato de cada ruta.

## 💡 Aprendizaje clave ##

- La automatización no reemplaza el criterio humano, lo potencia. Antes de crear un modelo, es fundamental comprender:
- Cómo están escritos los datos.
- Qué se quiere representar.
- Qué variaciones existen entre fuentes.
- Ese análisis previo es lo que permite que el modelo sea robusto, flexible y útil en contextos reales donde los datos nunca vienen perfectos.

## 🛠️ Herramientas utilizadas ##

QGIS – Modelador gráfico, procesamiento vectorial

Excel / CSV – Limpieza y estandarización de datos

GeoPackage – Almacenamiento de capas vectoriales

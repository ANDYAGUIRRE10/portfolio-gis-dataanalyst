# Conectividad y Accesibilidad Territorial — Distritos de Santa Fe

## Descripción del proyecto

Proyecto de análisis territorial orientado a explorar las diferencias en infraestructura vial, conectividad y contexto demográfico entre los distritos de la provincia de Santa Fe, Argentina.

El trabajo propone integrar información geográfica, vial y estadística para construir indicadores territoriales, comparar unidades espaciales y representar los resultados mediante cartografía temática.
Este se encuentra en etapa de planificación y desarrollo, incorporando herramientas de bases de datos espaciales, programación y análisis de datos.

## Objetivos

- Organizar e integrar información geográfica, vial y demográfica.
- Construir una base de datos espacial para almacenar y consultar los datos del proyecto.
- Calcular indicadores de infraestructura vial y conectividad a escala distrital.
- Explorar la relación entre población, superficie territorial y disponibilidad de infraestructura vial.
- Comparar distritos mediante estadísticas, indicadores y rankings.
- Elaborar mapas temáticos que faciliten la interpretación de los resultados.
- Documentar un flujo de trabajo reproducible que integre bases de datos, programación y herramientas GIS.

## Datos de trabajo

Las variables previstas para el análisis incluyen:

- **Límites y superficies distritales:** delimitación de las unidades espaciales de análisis.
- **Población por distrito:** información censal correspondiente al último censo disponible y a una fuente estadística documentada.
- **Longitud de rutas por distrito:** extensión de la infraestructura vial dentro de cada unidad territorial junto a otras características y atributos.
- **Nodos e intersecciones viales:** cantidad de cruces de la red vial, según criterios de identificación y validación que se definirán durante el desarrollo.

## Indicadores propuestos

Se evaluará la construcción de algunos indicadores como:

- Kilómetros de rutas por cada 100 km² de superficie distrital.
- Kilómetros de rutas por cada 1.000 habitantes.
- Cantidad de nodos o intersecciones viales por cada 100 km².
- Comparación y clasificación de distritos según las variables e indicadores calculados.

Los indicadores se interpretarán teniendo en cuenta las características territoriales y demográficas de cada distrito. Su finalidad será facilitar comparaciones exploratorias, no establecer por sí solos una medida definitiva de accesibilidad.

La accesibilidad efectiva a destinos específicos podrá abordarse en una etapa posterior, mediante información adicional sobre localidades, equipamientos y servicios, junto con métodos de análisis de redes cuando los datos disponibles lo permitan.

## Tecnologías previstas

| Tecnología | Aplicación en el proyecto |
|---|---|
| PostgreSQL | Almacenamiento y consulta de datos tabulares. |
| PostGIS | Gestión, consulta y procesamiento de datos espaciales. |
| SQL | Consultas, agregaciones, uniones y cálculo de indicadores. |
| Python | Automatización, preparación, validación y análisis de datos. |
| Pandas / GeoPandas | Procesamiento de tablas y datos geoespaciales. |
| VS Code | Desarrollo y organización del código. |
| Miniconda | Gestión del entorno y las dependencias de Python. |
| QGIS | Validación visual, análisis GIS y elaboración cartográfica. |
| Git / GitHub | Control de versiones, documentación y publicación del proyecto. |

Las tecnologías y librerías se incorporarán progresivamente según las necesidades del flujo de trabajo.

## Metodología de trabajo

1. **Revisión y preparación de datos:** identificación de fuentes, revisión de atributos, validación de geometrías y normalización de tablas.
2. **Organización de la información espacial:** estructuración de las capas y tablas necesarias para el análisis.
3. **Implementación de la base de datos:** creación de una base de datos PostgreSQL con soporte espacial mediante PostGIS.
4. **Integración y procesamiento:** carga de datos, consultas SQL, uniones espaciales y cálculo de variables derivadas.
5. **Construcción de indicadores:** cálculo, control y comparación de los indicadores territoriales seleccionados.
6. **Análisis exploratorio:** elaboración de estadísticas, tablas comparativas y rankings distritales.
7. **Representación cartográfica:** visualización y diseño de mapas temáticos en QGIS.
8. **Documentación y publicación:** organización del código, descripción de las fuentes, registro de decisiones metodológicas y publicación de los resultados en GitHub.

## Estructura prevista del repositorio

La estructura se ajustará a medida que se incorporen los componentes del proyecto.

```text
Conectividad_Accesibilidad_distritossantafe/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── sql/
├── notebooks/
├── scripts/
├── qgis/
├── outputs/
│   ├── tables/
│   └── maps/
└── docs/
```

Los datos originales, los resultados procesados, las consultas SQL, los scripts y las cartografías se organizarán de forma diferenciada para facilitar la trazabilidad del trabajo.

Los archivos de gran tamaño, los datos sensibles y las credenciales de conexión no se publicarán en el repositorio. Se documentarán las fuentes y las instrucciones necesarias para reproducir el flujo de trabajo cuando sea posible.

## Estado del proyecto

**En desarrollo — planificación metodológica y preparación del flujo de trabajo.**

Las tareas de implementación, procesamiento, cálculo de indicadores y producción cartográfica se documentarán conforme se completen.

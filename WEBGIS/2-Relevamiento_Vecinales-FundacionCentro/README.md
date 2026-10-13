# Seguimiento de relevamientos vecinales — Fundación Centro

## Sobre el proyecto

Proyecto de cartografía aplicada desarrollado para acompañar un plan de relevamiento de problemáticas barriales impulsado por Fundación Centro en la ciudad de Santa Fe.

La iniciativa contemplaba la realización de encuestas y reuniones con vecinos de las distintas vecinales para identificar problemáticas y necesidades territoriales. El área de trabajo comprendía 87 vecinales.

El trabajo cartográfico buscó representar el estado de avance de los relevamientos, diferenciando las vecinales ya relevadas de aquellas pendientes de intervención. De esta manera, se procuró ofrecer una visión espacial general que sirviera como apoyo para la planificación de las siguientes actividades de la fundación.

## Objetivos

- Representar geográficamente el avance del plan de relevamiento.
- Facilitar la identificación de vecinales relevadas y pendientes.
- Proporcionar una herramienta de consulta visual para acompañar la planificación territorial.
- Resolver una necesidad operativa concreta mediante una solución cartográfica de implementación sencilla y bajo requerimiento de infraestructura.

## Trabajo realizado

### 1. Recopilación y contraste de fuentes geográficas

Se recopilaron y contrastaron diversas fuentes de información para construir una representación de los límites de las vecinales de la ciudad.

La información municipal disponible presentaba limitaciones, con delimitaciones desactualizadas o incompletas, por lo que fue necesario consultar fuentes adicionales y realizar verificaciones para mejorar la consistencia de la cartografía utilizada.

### 2. Preparación y validación de datos espaciales

Se trabajó con datos vectoriales de las vecinales y sus atributos de estado de relevamiento.

En QGIS se revisaron las geometrías y se utilizaron reglas topológicas para detectar y corregir inconsistencias espaciales antes de elaborar la cartografía temática.

### 3. Diseño cartográfico

Se definió una simbología temática orientada a distinguir las vecinales según su estado de relevamiento.

El diseño priorizó la legibilidad y la identificación rápida de las áreas relevadas y pendientes, de acuerdo con las necesidades de consulta de la organización.

### 4. Publicación de un mapa web

Se utilizó el complemento QGIS2web para exportar la cartografía desde QGIS a una aplicación web estática.

La publicación mediante GitHub Pages permite compartir el mapa a través de un enlace web, sin necesidad de desplegar una base de datos espacial ni un servidor de mapas para esta implementación.

## Tecnologías y herramientas

- **QGIS:** preparación de datos, revisión de geometrías, validación topológica y diseño cartográfico.
- **QGIS2web:** exportación de la cartografía a un mapa web.
- **Leaflet:** biblioteca de mapas web, si corresponde al motor seleccionado en la exportación.
- **HTML, CSS y JavaScript:** componentes de la aplicación web generada.
- **GitHub y GitHub Pages:** alojamiento del código y publicación del mapa.

## Alcance y aporte profesional

Mi participación estuvo orientada a la recopilación y revisión de información geográfica, la validación de las geometrías, el diseño de la simbología y la construcción de una representación cartográfica para acompañar el trabajo de la fundación.

La selección de vecinales a relevar y el análisis de las problemáticas barriales correspondían a la organización. La cartografía tenía como finalidad facilitar la lectura territorial del avance y apoyar la planificación de futuras actividades.

El proyecto constituye un ejemplo de aplicación de herramientas GIS para responder a una necesidad concreta mediante una solución web sencilla, accesible y de bajo requerimiento de infraestructura.

## Estado del proyecto

Proyecto de cartografía aplicada con publicación web estática mediante QGIS2web y GitHub Pages.

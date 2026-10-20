## ⚽ 01: Dashboard de Rendimiento  - Liga MX (Apertura 2026)

**Objetivo:** Desarrollar un panel interactivo para el análisis de rendimiento colectivo e individual de los equipos de la Liga MX.
**Arquitectura y Origen de los Datos:**
* **Data Sourcing:** Extracción de datos estadísticos reales de partidos, jugadores y clasificación desde **FBref** (Sports Reference).
* **Modelado Relacional:** Transformación de datos crudos en un archivo estructurado compuesto por tablas de dimensiones (`equipos`, `jugadores`) y tablas de hechos (`jornadas`, `clasificacion`) para optimizar el modelo de datos en Power BI.

**Conceptos de Power BI aplicados:**
* **Modelado de Datos:** Relaciones de uno a muchos (1:*) entre catálogos de equipos/jugadores y las estadísticas de los partidos.
* **DAX y KPIs:** Creación de métricas compuestas (Goles + Asistencias, Participación G+A) para medir la productividad ofensiva.
* **Diseño UI/UX:** Implementación de segmentadores visuales (Slicers) personalizados con escudos de los clubes y maquetación tipo panel de control técnico.
* **Storytelling de Datos:** Tablas de clasificación dinámicas y gráficos de análisis de rendimiento frente a rivales directos.

**Conclusiones:** El panel permite a un cuerpo técnico o analista aislar instantáneamente el rendimiento de un club específico (ej. Club Puebla), visualizar a sus jugadores más determinantes en el ataque y contrastar la cantidad de goles anotados/recibidos dependiendo del rival en turno.

*(Consulta el archivo LigaMX2026.pdf incluido en esta carpeta para previsualizar el panel final).*

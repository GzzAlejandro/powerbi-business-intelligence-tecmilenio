## 🏈 02: Análisis Táctico de Series Ofensivas (Drives) - NFL (Temporada 2026)

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](#) [![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](#) [![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](#)

[NFLDashboard.pdf](https://github.com/user-attachments/files/34500396/NFLDashboard.pdf)


**Objetivo:** Desarrollar un panel de análisis interactivo enfocado en la eficiencia por serie ofensiva (drive), aislando el ruido estadístico de los boxscores tradicionales para evaluar la verdadera identidad táctica de las franquicias de la NFL.

**Arquitectura y Origen de los Datos:**
- **Data Sourcing:** Extracción y limpieza de registros transaccionales *play-by-play* (drives y estadísticas individuales) utilizando scripts de **Python (Pandas)** para depurar tiempos, categorizar los resultados de cada serie y consolidar la telemetría cruda.
- **Modelado Relacional:** Transformación de datos en un esquema de estrella estructurado, conectando catálogos dimensionales (`Equipos`, `Jugadores`, `Posiciones`) con tablas de hechos (`Jugadas_Equipos`, `Partidos`) y tablas agregadas (`Resumen_Jugadores`) para un filtrado cruzado impecable en Power BI.

**Conceptos de Power BI aplicados:**
- **Modelado Avanzado y DAX:** Uso de la función `SUMMARIZE` para crear tablas agregadas físicas y estabilizar el modelo de datos, evitando colisiones en los contextos de filtro al interactuar con el panel.
- **Filtros Top N Dinámicos:** Configuración matemática avanzada para aislar automáticamente al líder estadístico absoluto por categoría (Yardas, Intercepciones, Capturas) respetando el contexto cruzado de la franquicia seleccionada.
- **Diseño UI/UX:** Maquetación ejecutiva (Dark Mode) de alto contraste, incorporando una botonera personalizada con logotipos y una paleta semántica que destaca visualmente los errores críticos (rojo) frente a los aciertos (verde).
- **Storytelling de Datos:** Implementación de gráficos de dispersión con ejes temporales (reloj convertido a segundos continuos) para contrastar el ritmo vs. la explosividad, y mapas de calor (basados en volumen de jugadas) para exponer contundentemente el peligro del "3 y fuera".

**Conclusiones:** El panel permite a un cuerpo técnico o departamento de *scouting* evaluar en segundos el ADN de una ofensiva: identifica si un equipo es una aplanadora que controla el reloj de juego mediante marchas largas, o si depende de ataques aéreos explosivos. Al mismo tiempo, permite aislar con un clic a los jugadores más determinantes en el sistema de cualquier franquicia.

*(Consulta el archivo NFLDashboard.pdf incluido en esta carpeta para previsualizar el panel final en alta resolución).*

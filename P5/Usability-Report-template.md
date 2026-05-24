# Usability Report



<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRF017nhV-TFmNER2OM8UbXtdN6xwAKBYrv0i6onNfKu6Yn0BV0RK6aiOroeXl73LSY-B0&usqp=CAU" alt="usability Download png" style="height:150px" />

### Evaluación de usabilidad del proyecto  [Anime Ramen]

[24 de mayo de 2026]

[[Enlace a GITHUB del proyecto](https://github.com/JavierRG6/DIU1.HustleHard.git)]

### Realizado por: Wax&Wayne (DIU2)

En esta evaluación hemos analizado el proyecto de otro equipo aplicando técnicas de UX Research. Nuestra experiencia previa en evaluación de usabilidad se limita al marco académico de la asignatura, lo que nos ha permitido aplicar por primera vez de forma práctica herramientas como el Eye Tracking, el cuestionario SUS y la auditoría de accesibilidad


## 1 RESUMEN EJECUTIVO  (Executive Summary)

- **Objetivo:** El objetivo de esta evaluación es analizar la usabilidad y accesibilidad de Anime Ramen, una web de restaurante temático basada en el universo Ghibli, desarrollada por otro equipo de la asignatura. La evaluación se enmarca en un estudio A/B, donde nuestro propio diseño (Cafetería Fantasía) actúa como caso de comparación.
- **Metodología:** El estudio combina tres técnicas complementarias. En primer lugar, un A/B Testing entre-sujetos con 10 participantes distribuidos en dos grupos de 5. En segundo lugar, pruebas de Eye Tracking con GazeMapping para analizar el comportamiento visual de los usuarios. Por último, el cuestionario SUS (System Usability Scale) para medir la percepción subjetiva de usabilidad, complementado con una auditoría de accesibilidad mediante Lighthouse.
- **Principales Hallazgos:**
  - El botón de reserva principal (CTA) de Anime Ramen recibe una atención visual muy alta y está correctamente jerarquizado, lo que facilita la consecución del objetivo principal de la web.
  - La sección de biblioteca de Cafetería Fantasía es prácticamente ignorada por los usuarios, lo que refleja un problema de jerarquía de contenidos en nuestro propio diseño.
  - Anime Ramen presenta problemas de contraste en las tarjetas de los biomas que afectan a usuarios con baja visión, incumpliendo el criterio WCAG 1.4.3.
- **Resultado Global:** Anime Ramen obtiene una puntuación SUS media de 75.5, lo que lo sitúa en la categoría "Good" de la escala. Cafetería Fantasía obtiene 64.0, en la categoría "OK". Anime Ramen supera a nuestro diseño en usabilidad percibida y se sitúa en el percentil 74 de los sistemas evaluados con SUS a nivel global.


## 2. Metodología y Reclutamiento

[Describe el "cómo"]

- **Perfil de los participantes:** Resumen de la tabla demográfica (edad media, nivel digital).
- **Escenario de la prueba:** Descripción de las tareas que realizaron los usuarios.
- **Herramientas:** Mención de **GazeMapping**, Tally y herramientas de accesibilidad.

## 3. Resultados del Cuestionario SUS (Datos Cuantitativos)

[Aquí se muestran datos del análisis multivariable de SUS] 

- **Comparativa A vs. B:** Un gráfico de barras comparando la puntuación final de ambos diseños.
- **Desglose por ítems:** Identifica qué preguntas del SUS tuvieron peor puntuación (por ejemplo, si la pregunta 2 sobre "complejidad" fue muy alta en el Diseño B).

Valoración numérica del SUS - 


## 4. Análisis de Eye Tracking (Datos Biométricos)

[Presenta la evidencia visual del comportamiento del usuario]

- **Heatmaps (Mapas de calor):** Incluye las capturas de GazeMapping. Comenta si los usuarios miraron los **POI** (Puntos de Interés) definidos.
- **Zonas de Silencio:** Identifica elementos importantes que fueron totalmente ignorados.
- **Hallazgo clave:** Ejemplo: "El 80% de los usuarios ignoró el botón de CTA debido a su ubicación en el margen inferior".

## 5. Auditoría de Accesibilidad

Sintetiza el cumplimiento técnico y normativo.

- **Puntuación Automática:** (Lighthouse/WAVE).
- **Principales barreras:** Lista los errores críticos (contraste, falta de etiquetas, etc.) y cómo afectan a los usuarios con discapacidad.

## 6. Conclusiones y Recomendaciones (Actionable Insights)

No te limites a decir qué está mal; di cómo arreglarlo. Clasifica las recomendaciones por prioridad:

| **Prioridad**      | **Hallazgo**                                                 | **Recomendación de Mejora**                                  |
| ------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Alta (Crítica)** | Ej. El SUS indica alta complejidad y el Eye Tracking muestra confusión en el menú. | Simplificar la arquitectura de información y aumentar el tamaño de las fuentes. |
| **Media**          | Ej. Los usuarios no ven el botón de registro rápidamente.        | Cambiar el color del CTA a uno de mayor contraste según WCAG. |
| **Baja**           | Ej. El logo no redirige a la home.                               | Añadir el enlace estándar al logotipo en la cabecera.        |




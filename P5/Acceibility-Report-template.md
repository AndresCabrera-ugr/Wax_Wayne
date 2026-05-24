# Accesibility Report (template)

<img src="https://img.uxcel.com/cdn-cgi/image/format=auto/practices/wcag-principles-overview-1742315821212/a-1742315821212-2x.jpg" alt="usability Download png" style="height:200px" />

## 1. Ficha Técnica del Informe

Antes de entrar en detalles, define el alcance.

- **Nombre del proyecto:** Anime Ramen (Caso B)
- **Normativa de referencia:** WCAG 2.1, Nivel AA. Referencia: norma UNE-EN 301549.
- **Herramientas utilizadas:** Lighthouse (Google Chrome DevTools)
- **Fecha de la auditoría:** 24 de mayo de 2026

## 2. Puntuaciones Globales (Métricas Automáticas)

- Lighthouse Accessibility Score: 88/100
La puntuación de 88 sobre 100 indica un nivel de accesibilidad generalmente bueno. Lighthouse detectó 2 errores automáticos y 10 elementos adicionales que requieren comprobación manual. La herramienta superó 10 auditorías sin problemas. Hay que tener en cuenta que las herramientas automáticas solo detectan una parte de los problemas reales de accesibilidad, por lo que esta puntuación debe interpretarse como un punto de partida y no como una garantía de accesibilidad completa.

## 3. Análisis por Principios (POUR)

Para que el informe sea profesional, agrupa los fallos según los 4 principios de la accesibilidad:

<img src="https://cdn.sanity.io/images/r115idoc/production/e745ae232e5e6760c1392354021aed4eecc4627d-1920x1080.png" alt="usability Download png" style="height:200px" />

### A. Perceptible

- **Hallazgo:** Contraste insuficiente entre el texto y el fondo en las tarjetas de los cuatro biomas y en el footer. El texto con color #F4ECD8 sobre los fondos de color de cada tarjeta no alcanza el ratio mínimo de 4.5:1 exigido por el nivel AA. Afecta a etiquetas como "BIOMA 01", "EN CARTA AHORA" y a los enlaces del footer.
- **Impacto:** Los usuarios con baja visión o daltonismo pueden tener dificultades para leer estos contenidos, especialmente en condiciones de luz ambiental alta.
- **Solución:** Aumentar el contraste del texto en las tarjetas oscureciendo el fondo o cambiando el color del texto a un tono más claro que supere el ratio 4.5:1. Herramientas como el Colour Contrast Analyser permiten validar la combinación de colores antes de implementarla.



### B. Operable

- **Hallazgo:** No se han detectado errores críticos de operabilidad mediante herramienta automática. La web no contiene elementos con tiempo limitado ni destellos que puedan causar convulsiones. Sin embargo, no se ha podido verificar manualmente la navegación completa por teclado.
- **Impacto:** Bajo en términos automáticos, aunque se recomienda una revisión manual de la navegación por teclado para confirmar que todos los elementos interactivos son accesibles sin ratón.
- **Solución:** Realizar una prueba manual de navegación con la tecla Tab para verificar que el foco es visible en todos los elementos interactivos y que el orden de tabulación es lógico.



### C. Comprensible

- **Hallazgo:** No se detectaron errores automáticos en este principio. El idioma de la página está correctamente definido en el HTML, lo que permite a los lectores de pantalla utilizar la pronunciación correcta.
- **Impacto:** Ninguno detectado automáticamente.
- **Solución:** Se recomienda verificar manualmente que los formularios de reserva incluyen etiquetas claras y mensajes de error descriptivos en caso de fallo de validación.



### D. Robusto

- **Hallazgo:** El documento HTML no define un elemento main, que es el landmark semántico que indica a los lectores de pantalla dónde empieza el contenido principal de la página.
- **Impacto:** Un usuario que navegue con lector de pantalla no puede saltar directamente al contenido principal y se ve obligado a recorrer toda la cabecera y navegación cada vez que carga la página, lo que resulta especialmente frustrante en visitas recurrentes.
- **Solución:** Envolver el contenido principal de la página en una etiqueta <main>. Es un cambio de una sola línea de código con un impacto directo y significativo para usuarios de tecnologías de asistencia.
  

## 4. Tabla de Hallazgos y Prioridades

Organiza los errores técnicos de forma que el equipo sepa qué arreglar primero.

| **ID**     | **Prioridad** | **Criterio WCAG**          | **Error detectado**                  | **Recomendación Técnica**     |
| ---------- | ------------- | -------------------------- | ------------------------------------ | ----------------------------- |
| **ACC-01** | **Crítica**   | 1.4.3 Contraste mínimo     | Texto #F4ECD8 sobre fondos de color en tarjetas de biomas y footer | Ajustar combinación de colores hasta superar ratio 4.5:1 en todos los elementos |
| **ACC-02** | **Alta**      |4.1.2 Nombre, función, valor| Ausencia de landmark main en el documento HTML      |Envolver el contenido principal en una etiqueta <main>|
| **ACC-03** | **Media**     | 2.4.3 Orden del foco       | No verificado manualmente: posible foco invisible en navegación |Revisar navegación por teclado y definir estilos CSS para :focus con contraste|







## 5. Conclusiones y Declaración de Conformidad

Resume el estado actual:

- **¿Es el sitio accesible?** (Ej: "El sitio cumple parcialmente con el nivel AA, pero presenta barreras críticas en el proceso de compra").
- **Próximos pasos:** Lista de 3 acciones inmediatas para mejorar la puntuación.














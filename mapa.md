# El mapa: cada paso de la investigación, ¿con IA?

De 27 pasos de una investigación empírica, 11 se pueden delegar con auditoría, 7 admiten a la IA como asistente o crítico y 9 son solo tuyos. La columna "Cómo auditarlo" es la que convierte un paso delegado en un paso aceptable.

- **Delegable con auditoría:** la IA (o un agente) lo ejecuta; tú revisas el resultado con el método de la última columna.
- **Asistente o crítico:** la IA propone, explica o critica; la decisión y el texto final son tuyos.
- **Solo tú:** puedes conversarlo con la IA, pero el producto sale de tu cabeza y de tu mano.

| Etapa | Paso | ¿Con IA? | Cómo usarla | Cómo auditarlo |
| --- | --- | --- | --- | --- |
| Planteamiento | Elegir tema y pregunta | Solo tú | Lluvia de ideas a partir de quién eres, qué sabes y a quién conoces ([flujo 2](flujos/flujo-2.md)). La IA propone; tú eliges. | ¿Puedes explicar en dos minutos, sin notas, por qué esta pregunta importa? |
| Planteamiento | Vaciar tus ideas en crudo | Delegable con auditoría | Dicta sin filtro; la IA transcribe y ordena ([flujo 1](flujos/flujo-1.md)). | Lo ordenado conserva tus ideas y no agrega otras. |
| Planteamiento | Planteamiento del problema | Asistente o crítico | Revisor que detecta cuando metes la solución dentro del problema ([flujo 3](flujos/flujo-3.md)). | La oración final la escribes tú. |
| Planteamiento | Objetivos, hipótesis y preguntas | Asistente o crítico | Crítico de coherencia: ¿cada objetivo responde a una pregunta y cada pregunta a una hipótesis? | Tu asesor entiende el plan en una cuartilla. |
| Literatura | Búsqueda de literatura | Delegable con auditoría | Investigación profunda o un agente con búsqueda académica ([flujo 4](flujos/flujo-4.md)). | Cada referencia: que exista (DOI), que la hayas abierto y que diga lo que dices que dice. |
| Literatura | Leer y comprender artículos | Asistente o crítico | NotebookLM: resumen en audio, mapa mental, preguntas al documento (Bonus). | Los 5 a 10 artículos clave los lees completos tú. |
| Literatura | Matriz de literatura (autor, método, resultado) | Delegable con auditoría | Tabla generada desde los PDF que tú subiste. | Cada celda trae página o sección citable; revisas una muestra. |
| Literatura | Marco teórico (el argumento) | Solo tú | Mapa de teorías, conceptos y contraargumentos ([flujo 4](flujos/flujo-4.md)). | Defiendes tu hipótesis frente a la teoría alternativa sin apoyo. |
| Diseño | Estrategia de identificación o diseño del estudio | Solo tú | Pídele las amenazas a la validez de tu diseño, no el diseño. | Puedes justificar cada supuesto ante el comité. |
| Diseño | Diseño de instrumento | Asistente o crítico | Borrador de reactivos a partir de tus subíndices y variables ([flujo 5](flujos/flujo-5.md)). | Validación con expertos y piloto con personas reales. |
| Diseño | Formulario o plataforma de captura | Delegable con auditoría | Script de Google Apps Script, formulario o página web ([flujo 7](flujos/flujo-7.md)). | Lo llenas tú completo y revisas la base que genera. |
| Datos | Trabajo de campo y entrevistas | Solo tú | Solo logística: rutas, recordatorios, transcripción con consentimiento. | Tu bitácora de campo. |
| Datos | Respuestas "sintéticas" generadas por IA | Solo tú | Nunca como datos. Solo para pilotear la redacción de preguntas. | No aparecen en ninguna tabla de resultados. |
| Datos | Entender la metodología de una fuente (p. ej. ENOE) | Delegable con auditoría | Sube el documento metodológico y hazle preguntas ([flujo 6](flujos/flujo-6.md)). | Cada dato clave (muestra, error, definiciones) lo ubicas en el documento. |
| Datos | Descarga, limpieza y unión de bases | Delegable con auditoría | Un agente escribe un script reproducible ([flujo 6](flujos/flujo-6.md)). | Conteo de observaciones antes y después de cada paso; revisas los descartes. |
| Datos | Estadística descriptiva y gráficas | Delegable con auditoría | Siempre desde código, nunca imágenes generadas. | Comparas con cifras publicadas que conoces (INEGI, Banxico). |
| Análisis | Especificación del modelo | Solo tú | Que te liste alternativas y supuestos; tú eliges y justificas. | Escribiste qué esperabas encontrar antes de correrlo. |
| Análisis | Estimación y código econométrico | Delegable con auditoría | Un agente programa y corre; tú especificas ([flujo 6](flujos/flujo-6.md)). | Replicas a mano una estimación clave; lees el código línea por línea. |
| Análisis | Robustez y replicación | Delegable con auditoría | Agentes para reproducir y variar especificaciones. | Sabes qué cambió en cada prueba y por qué. |
| Análisis | Interpretación de resultados | Solo tú | Pregúntale qué otras explicaciones podría tener el resultado. | Interpretas la tabla en vivo, sin apoyo. |
| Escritura | Redacción del texto | Solo tú | No. | La prueba de la revelación (ver [Qué es recomendable y qué no](que-es-recomendable.md)). |
| Escritura | Revisión de estilo y ortografía | Asistente o crítico | Que señale problemas, no que reescriba ([flujo 8](flujos/flujo-8.md)). | Tú aplicas cada cambio a mano. |
| Escritura | Formato de referencias (APA) | Delegable con auditoría | A partir de la URL o el DOI. | Cotejas autor, año y revista contra la fuente. |
| Escritura | Traducción del resumen | Asistente o crítico | Tú lo escribes en español; la IA traduce. Paso debatible. | Revisas cada término técnico. |
| Escritura | Revisión previa tipo dictamen | Asistente o crítico | Revisor adversarial que busca fallas ([flujo 8](flujos/flujo-8.md)). | Tú decides qué atender y por qué. |
| Difusión | Presentación, sitio o tablero | Delegable con auditoría | Diapositivas, página web, dashboard ([flujo 7](flujos/flujo-7.md)). | Cada número coincide con tu tesis. |
| Difusión | Declaración de uso de IA | Solo tú | — | Plantilla en los Bonus. |

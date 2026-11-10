# Flujo 6. Datos y econometría con agentes

Un agente (Claude Code, Codex, Gemini CLI, o el modo de análisis de datos de cualquier chat) puede descargar datos, limpiarlos, correr la regresión, hacer las gráficas y corregir sus propios errores. Yo lo he usado para construir cuadernos de Python para mis alumnos, scripts de limpieza, gráficas de modelos económicos y tablas de comparación de modelos. Tu trabajo cambia de *ejecutar* a *especificar y auditar*.

**Paso 0: entiende la fuente antes de tocar los datos.** Si no capturaste los datos, tienes que conocer su metodología como si lo hubieras hecho. Sube el documento metodológico (p. ej. "Cómo se hace la ENOE" del INEGI):

```txt
Estoy haciendo un estudio sobre {tema}. Lee con atención el documento metodológico adjunto y descríbeme:
- El diseño estadístico: tamaños de muestra, confianza y error.
- Las limitaciones del diseño, incluida la representatividad.
- Aspectos del levantamiento a considerar.
- Definiciones clave.
- Variables clave para mi análisis, incluidas las de control.
Cita la página o sección de cada afirmación.
```

**El flujo con un agente:**

1. **Escribe tú el plan de análisis** (media cuartilla): pregunta, fuente, unidad de observación, variable dependiente, variables explicativas, modelo y **qué esperas encontrar**.
2. **Pídele un script, no un resultado.** Todo en un archivo `.R` o `.py` que se pueda correr de principio a fin, con comentarios.
3. **Revisa los pasos intermedios.** Observaciones antes y después de cada filtro, variables creadas, valores faltantes, una tabla descriptiva que puedas comparar con cifras publicadas.
4. **Lee el código** del modelo línea por línea. Si no entiendes una línea, pregunta hasta entenderla.
5. **Compara con tu predicción.** Si el resultado te sorprende, primero sospecha de los datos, después del código y al final de tu teoría.
6. **Replica a mano** una estimación clave.

```txt
Eres mi asistente de investigación en econometría. Este es mi plan de análisis: {pega tu plan}.
Reglas:
1. Todo en un script reproducible en {R / Python}, comentado en español. Nada de cálculos fuera del script.
2. Después de cada paso de limpieza, reporta cuántas observaciones quedan y por qué se eliminaron las demás.
3. Antes de estimar, muéstrame la estadística descriptiva y detente para que yo la revise.
4. No cambies la especificación del modelo sin preguntarme. Si crees que hay un problema (endogeneidad, multicolinealidad, errores estándar), dime cuál y por qué, y yo decido.
5. Las gráficas se generan desde el código y se guardan como archivos.
```

La regla 3 es la más importante: un agente sin pausas te entrega un resultado terminado que no tienes forma de revisar.

!!!secondary Para saber más: Lo que la IA ya puede hacer en ciencias sociales

- **Reproducir artículos.** Con los datos y el código originales, agentes como Claude Code y Codex reprodujeron gran parte de los resultados de 54 artículos de ciencias sociales ([Alizadeh et al., 2026](https://arxiv.org/html/2606.11447)). Con solo el texto de métodos y los datos, sin el código, también los recuperaron en muchos casos ([Kohler et al., 2026](https://arxiv.org/html/2604.21965v2)). Y ya hay una prueba a ciegas de un agente que detecta errores sembrados en paquetes de replicación de economía ([Zhang y Zhu, 2026](https://www.sciencedirect.com/science/article/abs/pii/S0165176526004623)).
- **Predecir experimentos.** En 70 experimentos de encuesta en EE. UU., las predicciones de GPT-4 se correlacionaron fuertemente con los efectos reales, con precisión similar a la de pronósticos humanos, aunque sobreestimó el tamaño de los efectos ([Hewitt, Ashokkumar et al., Nature](https://www.gsb.stanford.edu/faculty-research/publications/large-language-models-can-predict-results-social-science-experiments)).
- **Encuestados sintéticos: no.** Pew Research probó si la IA puede sustituir a encuestados reales; su respuesta fue "no realmente", con errores promedio de 11 a 16 puntos porcentuales ([Pew, 2026](https://www.pewresearch.org/data-labs/2026/09/30/methodology-silicon-samples/)). Sirven para pilotear un instrumento, nunca como datos.
- **Escribir artículos completos.** *The AI Scientist* genera ideas, programa, corre experimentos, escribe el manuscrito y se revisa a sí mismo ([Lu et al., 2026, Nature](https://ora.ox.ac.uk/objects/uuid:92d16200-fbe1-4564-b4d4-694e96223b39)). Que se pueda no significa que sea recomendable en una tesis (ver [Qué es recomendable y qué no](../que-es-recomendable.md)).
!!!

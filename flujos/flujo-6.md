# Flujo 6. Datos y econometría con agentes

**Para qué sirve:** analizar tus datos con ayuda de la IA sin perder el control: que ella programe y tú especifiques y revises. **Tiempo:** 1 hora para el ejercicio; tu análisis real, lo que tome. **Herramienta:** Claude (la versión gratuita ejecuta código y acepta archivos), el análisis de datos de ChatGPT (limitado en la gratuita) o Google Colab con Gemini.

## Un error de Excel que movió la política económica de medio mundo

En 2010, Carmen Reinhart y Kenneth Rogoff publicaron un estudio que se volvió famosísimo: los países con una deuda pública mayor al 90 % de su PIB crecían mucho menos. Políticos de varios países lo citaron para justificar recortes de gasto.

En 2013, un estudiante de doctorado de la Universidad de Massachusetts intentó replicarlo como tarea y no le cuadraban los números. Encontró, entre otras cosas, un error en la hoja de cálculo: una fórmula de promedio dejaba fuera a cinco países. Con los datos corregidos, el crecimiento promedio de los países muy endeudados no era negativo, sino de 2.2 % (Herndon, Ash y Pollin, 2014).

No te cuento esto para burlarme de dos economistas brillantes. Te lo cuento porque **a cualquiera le pasa**. Cuando economistas intentaron replicar 67 artículos publicados en revistas importantes usando los datos y el código de los autores, solo pudieron reproducir el resultado principal de una tercera parte sin pedirles ayuda (Chang y Li, 2022).

Si eso pasa con investigadores profesionales, imagina un análisis que nadie más puede revisar porque vive en clics sueltos.

## La IA puede hacer todo el análisis. Ese es justo el riesgo.

Hoy un **agente** (una IA que usa herramientas por su cuenta: escribe código, lo corre, ve el error y lo corrige) puede descargar datos, limpiarlos, correr la regresión y hacer las gráficas. Yo lo he usado para construir cuadernos de Python para mis alumnos, scripts de limpieza y tablas de comparación de modelos.

Tu trabajo cambia de **ejecutar** a **especificar y auditar**. Y aquí está la trampa: un agente sin pausas te entrega un resultado terminado, con buena presentación, que no tienes forma de revisar. Es un Reinhart-Rogoff esperando a pasar.

La IA tiene conocimiento de doctorado. Pero recuerda que el doctorado no quita lo tarado: puede eliminar observaciones sin avisarte, cambiar tu modelo "porque se ve mejor" o interpretar un coeficiente al revés.

## Pídele un script, no un resultado

La regla que lo cambia todo: que **todo** el análisis viva en un archivo de código (R o Python) que se pueda correr de principio a fin. Así:

- **Se puede revisar.** Cada decisión (qué observaciones quitaste, qué variables creaste) está escrita.
- **Se puede repetir.** Si mañana te llegan datos nuevos, corres el mismo script.
- **Se puede defender.** Ante tu comité, el script es tu evidencia de que el número no salió de la nada.

Los errores típicos son tres: pedir "analiza mis datos" sin decir qué esperas encontrar; aceptar el número final sin mirar los pasos intermedios; y dejar que la IA cambie tu especificación sin preguntarte.

## Una hora, seis pasos

>>> 0. Entiende la fuente antes de tocar los datos
Si no levantaste los datos tú, tienes que conocer su metodología como si lo hubieras hecho. Sube el documento metodológico (por ejemplo, "Cómo se hace la ENOE" de INEGI):

```txt
Estoy haciendo un estudio sobre {tema}. Lee con atención el documento metodológico adjunto y descríbeme:
- El diseño estadístico: tamaños de muestra, confianza y error.
- Las limitaciones del diseño, incluida la representatividad.
- Aspectos del levantamiento a considerar.
- Definiciones clave.
- Variables clave para mi análisis, incluidas las de control.
Cita la página o sección de cada afirmación.
```

"Cita la página" te deja comprobar cada afirmación en segundos.
>>>

>>> 1. Escribe tú el plan de análisis
Media cuartilla: pregunta, fuente, unidad de observación, variable dependiente, variables explicativas, modelo y **qué esperas encontrar**. Esa última línea es tu detector de errores: si el resultado sale muy distinto, algo hay que revisar.
>>>

>>> 2. Dale reglas al agente
```txt
Eres mi asistente de investigación en econometría. Este es mi plan de análisis: {pega tu plan}.
Reglas:
1. Todo en un script reproducible en {R / Python}, comentado en español. Nada de cálculos fuera del script.
2. Después de cada paso de limpieza, reporta cuántas observaciones quedan y por qué se eliminaron las demás.
3. Antes de estimar, muéstrame la estadística descriptiva y detente para que yo la revise.
4. No cambies la especificación del modelo sin preguntarme. Si crees que hay un problema (endogeneidad, multicolinealidad, errores estándar), dime cuál y por qué, y yo decido.
5. Las gráficas se generan desde el código y se guardan como archivos.
```

La regla 3 es la más importante: es la pausa que te deja revisar antes de que haya un resultado que te guste.
>>>

>>> 3. Revisa los pasos intermedios
Observaciones antes y después de cada filtro, variables creadas, valores faltantes. Compara la estadística descriptiva con cifras publicadas: si tu salario promedio no se parece al que reporta INEGI para esa población, algo anda mal.
>>>

>>> 4. Lee el código del modelo
Línea por línea. Si no entiendes una línea, pregunta hasta entenderla. No necesitas saber programar para esto; necesitas saber qué debería estar haciendo cada paso.
>>>

>>> 5. Compara con tu predicción y replica algo a mano
Si el resultado te sorprende, primero sospecha de los datos, después del código y al final de tu teoría. Y replica a mano (o en otra herramienta) al menos una estimación clave.
>>>

## "Sí, pero…"

**"No sé programar."** No necesitas escribir el código, pero sí leerlo. Pídele a la IA que te explique cada bloque en español. Con el tiempo vas a reconocer los patrones, igual que aprendiste a leer una tabla de regresión.

**"¿R o Python?"** El que use tu asesor o tu área. Los dos son software libre y la IA maneja muy bien ambos.

**"La versión gratuita se me corta a media sesión."** Por eso el script: si se corta, abres otra conversación, subes el script y los datos, y sigues donde te quedaste. Es otra razón para no depender de la memoria del chat.

**"¿Y Claude Code, Codex y esos agentes de los que todos hablan?"** Son la versión más poderosa de este flujo: trabajan directamente sobre las carpetas de tu computadora, corren análisis completos y pueden pasar horas en una tarea. Requieren plan de pago y algo de configuración. Para empezar, el chat gratuito con ejecución de código es suficiente.

## Míralo funcionar (y pruébalo tú)

Preparé una base de **datos simulados** para que practiques: [salarios-simulados.csv](/static/datos/salarios-simulados.csv). Son 1,000 personas con salario mensual, años de educación, experiencia, sexo y el puntaje en una prueba de habilidades.

Como la simulé yo, sé la respuesta: **cada año de educación aumenta el salario 8 %**. Pero metí tres trampas, como en los datos reales:

1. Hay salarios faltantes.
2. Hay dos capturas absurdas (un salario de 9,999,999).
3. La habilidad influye en el salario y también en cuántos años estudias. Si no la controlas (con el puntaje de la prueba), el efecto de la educación sale inflado. Es el **sesgo por variable omitida**.

Un buen análisis debería reportarte las tres cosas y llegar a un efecto cercano a 8 %. Uno descuidado te va a dar alrededor de 11 % y no te va a avisar de nada.

## Tu turno

!!!success 1 hora, ¿encontraste las trampas?
1. Descarga [salarios-simulados.csv](/static/datos/salarios-simulados.csv) y súbelo a tu chat.
2. Escribe un plan de análisis de cinco líneas: pregunta, variables, modelo (regresión del logaritmo del salario) y qué esperas encontrar.
3. Usa el *prompt* del paso 2.
4. Revisa: ¿te reportó los faltantes? ¿Detectó las dos capturas absurdas? ¿Te sugirió controlar por habilidad, o te preguntó antes de agregarla?
5. Compara su resultado con el 8 % verdadero.

Si te dio 11 % sin decir nada, ya viste por qué la regla 3 existe.
!!!

!!!secondary Para saber más: Lo que la IA ya puede hacer en ciencias sociales
- **Reproducir artículos.** Con los datos y el código originales, agentes como Claude Code y Codex reprodujeron gran parte de los resultados de 54 artículos de ciencias sociales ([Alizadeh et al., 2026](https://arxiv.org/html/2606.11447)). Con solo el texto de métodos y los datos, sin el código, también los recuperaron en muchos casos ([Kohler et al., 2026](https://arxiv.org/html/2604.21965v2)). Y ya hay una prueba a ciegas de un agente que detecta errores sembrados en paquetes de replicación de economía ([Zhang y Zhu, 2026](https://www.sciencedirect.com/science/article/abs/pii/S0165176526004623)).
- **Predecir experimentos.** En 70 experimentos de encuesta en EE. UU., las predicciones de GPT-4 se correlacionaron fuertemente con los efectos reales, con precisión similar a la de pronósticos humanos, aunque sobreestimó el tamaño de los efectos ([Hewitt, Ashokkumar et al., Nature](https://www.gsb.stanford.edu/faculty-research/publications/large-language-models-can-predict-results-social-science-experiments)).
- **Encuestados sintéticos: no.** Pew Research probó si la IA puede sustituir a encuestados reales; su respuesta fue "no realmente", con errores promedio de 11 a 16 puntos porcentuales ([Pew, 2026](https://www.pewresearch.org/data-labs/2026/09/30/methodology-silicon-samples/)). Sirven para pilotear un instrumento, nunca como datos.
- **Escribir artículos completos.** *The AI Scientist* genera ideas, programa, corre experimentos, escribe el manuscrito y se revisa a sí mismo ([Lu et al., 2026, Nature](https://ora.ox.ac.uk/objects/uuid:92d16200-fbe1-4564-b4d4-694e96223b39)). Que se pueda no significa que sea recomendable en una tesis (ver [Qué es recomendable y qué no](../que-es-recomendable.md)).
!!!

!!!primary Cuando quieras trabajar con agentes de verdad
Todo este flujo funciona con la versión gratuita de un chat. El siguiente nivel son agentes como **Claude Code**, que trabajan sobre las carpetas de tu proyecto, corren análisis completos y dejan todo documentado. En mi comunidad **Economista Full Stack** comparto los scripts, plantillas y *prompts* que uso, y en las sesiones semanales puedes traer tu propio proyecto. Tienes **7 días gratis** para probarla y cancelas cuando quieras.

[!button variant="primary" text="Probar 7 días gratis"](https://www.skool.com/economista-full-stack-6510/about)
!!!

## Referencias de este flujo

- Chang, A. C. y Li, P. (2022). Is economics research replicable? Sixty published papers from thirteen journals say "often not". *Critical Finance Review*, 11(1), 185–206.
- Herndon, T., Ash, M. y Pollin, R. (2014). Does high public debt consistently stifle economic growth? A critique of Reinhart and Rogoff. *Cambridge Journal of Economics*, 38(2), 257–279.

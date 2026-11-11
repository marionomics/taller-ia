---
label: "Qué IA usar"
order: 850
icon: tools
---
# Qué IA usar (y qué puedes hacer gratis)

"¿Cuál es la mejor IA?" es la pregunta que más me hacen en los talleres. La respuesta corta te va a decepcionar: cualquiera de las tres grandes. La respuesta larga es más útil, porque lo que de verdad cambia tus resultados no es la marca, sino **qué modelo** usas y **en qué modo**.

## Cualquiera de las tres grandes te sirve

Los tres jugadores principales son **OpenAI** (ChatGPT), **Google** (Gemini) y **Anthropic** (Claude). Se turnan el primer lugar cada pocos meses, así que no te voy a dar nombres de versiones: estarían viejos cuando leas esto. Si quieres ver quién va arriba hoy, revisa un ranking independiente como [Artificial Analysis](https://artificialanalysis.ai/).

Prefiero los modelos generales sobre las herramientas "especializadas" para tesis que ves anunciadas. La mayoría son una máscara sobre alguno de los tres grandes, con un *prompt* ya escrito. Y estar entrenado en un tema no garantiza ganar: Bloomberg entrenó su propio modelo con décadas de información financiera, y GPT-4, un modelo general, lo superó en casi todas las tareas financieras que se probaron, sin entrenamiento especial (Li et al., 2023).

## Cada empresa tiene modelos grandes y modelos chicos

Dentro de cada marca hay una familia de modelos. Se parecen a los asistentes de un laboratorio:

- **Los modelos chicos** son rápidos y baratos. Son como el becario de primer semestre: perfecto para traducir algo, explicarte un término o darte cinco sinónimos.
- **Los modelos grandes** tardan más y cuestan más, pero razonan mejor y se equivocan menos. Son como el doctorante: a él le pides que revise la lógica de tu protocolo, no que te traduzca "hola mundo".

Además, casi todos tienen un **modo de razonamiento** (el botón dice "pensar", "razonar" o algo parecido). En ese modo, el modelo escribe primero un borrador de su razonamiento, paso a paso, y después te contesta. Tarda más, pero acierta más en lo que requiere lógica: revisar un argumento, resolver un problema de matemáticas, detectar contradicciones.

Una regla práctica:

| Si tu pregunta es… | Usa… | Ejemplo |
| --- | --- | --- |
| Rápida y sin mucho razonamiento | El modo rápido | "¿Qué es una variable instrumental?" |
| De lógica, revisión o varios pasos | El modo de razonamiento | "Revisa si mi hipótesis se sigue de mi marco teórico" |
| De búsqueda de muchas fuentes | Investigación profunda | "Encuentra estudios sobre el salario mínimo en México" |
| De trabajo con archivos y código | Análisis de datos o un agente | "Corre esta regresión con mi base de datos" |

Hay otro concepto que te conviene conocer: la **ventana de contexto**, que es cuánto texto puede "tener en mente" el modelo a la vez. Si quieres que revise tu tesis completa, importa. Las versiones gratuitas suelen tener ventanas más pequeñas: la de Gemini, por ejemplo, equivale a unas 50 páginas de texto ([9to5Google, 2026](https://9to5google.com/2026/05/25/google-ai-plus-pro-ultra-gemini-features/)). Si tu documento es más largo, dáselo por capítulos.

## Lo que la versión gratuita te da hoy

Todo lo que necesitas para los ocho flujos de esta guía se puede hacer gratis. Esto es lo que trae cada versión gratuita, revisado en noviembre de 2026 (los planes cambian seguido; confírmalo en las páginas de precios de [ChatGPT](https://chatgpt.com/pricing), [Gemini](https://gemini.google/subscriptions/) y [Claude](https://claude.com/pricing)):

| | ChatGPT | Gemini | Claude |
| --- | --- | --- | --- |
| Modelo | Su modelo pequeño, más un modo de razonamiento ligero | Su modelo rápido, con acceso limitado al grande | Sus modelos mediano y pequeño |
| Búsqueda en internet | Sí | Sí | Sí |
| Subir archivos | Limitado | Sí | Sí |
| Ejecutar código y analizar datos | Limitado | Con Google Colab | Sí |
| Investigación profunda | Algunas al mes | Algunas al mes | No (de pago) |
| Lienzo para documentos y herramientas | Canvas | Canvas | Artefactos |
| Proyectos con contexto permanente | De pago | Gems | Hasta 5 |
| Agentes de código | Codex, limitado | No | No (de pago) |

Y una más de Google que vale oro para leer artículos: **NotebookLM**, gratis con tu cuenta de Google. Le subes tus documentos y responde solo con base en ellos, con citas a la página.

## Qué herramienta para cada flujo

| Flujo | Lo mínimo que necesitas | Si tienes más |
| --- | --- | --- |
| [1. Vacía tus ideas](flujos/flujo-1.md) | Cualquier chat con dictado | — |
| [2. Ideas de investigación](flujos/flujo-2.md) | Cualquier chat | — |
| [3. Protocolo](flujos/flujo-3.md) | Chat con modo de razonamiento | Un Proyecto para tu tesis |
| [4. Bibliografía](flujos/flujo-4.md) | Investigación profunda (Gemini o ChatGPT) + Google Scholar + NotebookLM | Investigación profunda sin límites |
| [5. Instrumento](flujos/flujo-5.md) | Cualquier chat | — |
| [6. Datos](flujos/flujo-6.md) | Claude o ChatGPT con análisis de datos, o Google Colab con Gemini | Un agente como Claude Code |
| [7. Artefactos](flujos/flujo-7.md) | Artefactos de Claude o Canvas de Gemini | Un agente para herramientas más grandes |
| [8. Revisor](flujos/flujo-8.md) | Chat con modo de razonamiento | Un modelo grande |

## ¿Vale la pena pagar?

Ponte el sombrero de economista: entrenar y operar estos modelos cuesta muchísimo. Si el servicio es gratis, el producto eres tú. En las versiones gratuitas, tus conversaciones pueden usarse para entrenar los modelos; casi todas tienen una opción en la configuración para desactivarlo. Revísala.

Mi recomendación: **empieza gratis**. Cuando llegues a una etapa intensa de tu investigación (la revisión de literatura, el análisis de datos), paga un mes de la herramienta que más estés usando. Con el plan de pago obtienes modelos más grandes, más uso antes de toparte con el límite, investigación profunda sin racionar y agentes. Cuando termine esa etapa, cancela si quieres.

## Lo que no te da ningún plan

Le pueden hacer todas las mejoras que quieran a la IA, pero mientras tú no sepas bien lo que quieres, no te va a dar grandes resultados. Es como tener un Ferrari y negarte a aprender a manejar estándar.

Tu ventaja no la vas a ganar pagando el modelo más caro. La ganas con claridad de pensamiento: sabiendo qué preguntas, por qué y cómo vas a revisar la respuesta. Eso es lo que practicas en cada flujo.

!!!primary El siguiente nivel: agentes
Cuando domines los flujos con la versión gratuita, el siguiente paso son los agentes como **Claude Code**, que trabajan directamente sobre las carpetas de tu proyecto. En mi comunidad **Economista Full Stack** comparto los scripts, plantillas y *prompts* que uso, y en las sesiones semanales puedes traer tu propio proyecto. Tienes **7 días gratis** para probarla y cancelas cuando quieras.

[!button variant="primary" text="Probar 7 días gratis"](https://www.skool.com/economista-full-stack-6510/about)
!!!

## Referencias de esta sección

- Li, X., Chan, S., Zhu, X., Pei, Y., Ma, Z., Liu, X. y Shah, S. (2023). Are ChatGPT and GPT-4 general-purpose solvers for financial text analytics? A study on several typical tasks. *Proceedings of EMNLP 2023: Industry Track*. arXiv:2305.05862.

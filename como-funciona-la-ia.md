# Cómo funciona la IA (lo mínimo para usarla bien)

ChatGPT, Gemini y Claude son **modelos de lenguaje**: modelos estadísticos entrenados con casi todo lo que la humanidad ha escrito, que predicen cuál es la siguiente palabra más probable. Si le pides ideas para visitar la Ciudad de México, la respuesta más probable empieza con "ir al Zócalo", no con "comer tacos al pastor". Saber esto explica casi todos los errores que vas a ver en el taller:

- **No es un buscador.** No consulta una base de datos: genera lo que suena probable. Por eso puede inventar una referencia con total seguridad (a esto se le llama *alucinación*). Pasa hasta a los expertos: en artículos aceptados en NeurIPS 2025, una de las conferencias más prestigiosas de IA, se encontraron 100 citas inventadas que ningún revisor detectó (Ansari, 2026). Toda cita se verifica en su fuente.
- **Es un promedio de lo escrito.** Si le pides "algo innovador" sin contexto, te dará lo más común. Y como casi todo lo escrito viene de países ricos y en inglés, razona desde ahí: sus respuestas se parecen más a las de personas de países occidentales y ricos (Atari et al., 2023), así que tu contexto se lo tienes que dar tú.
- **Está entrenada para agradarte.** Las personas que la calificaron preferían respuestas que les dieran la razón, así que tiende a confirmar lo que piensas (Sharma et al., 2024; Cheng et al., 2026). Si quieres crítica, pídela de forma explícita.

Hoy la puedes usar de cuatro formas, que siguen la evolución de chatbots a modelos de razonamiento y a agentes que describe [Korinek (2025)](https://www.nber.org/papers/w34202). Los tres grandes (ChatGPT, Gemini y Claude) tienen las cuatro:

| Modo | Qué hace | Úsalo para |
| --- | --- | --- |
| Chat rápido | Responde al momento | Preguntas simples: traducir, explicar un término |
| Razonamiento | "Piensa" varios pasos antes de responder | Revisar la lógica de tu protocolo o tu argumento |
| Investigación profunda (*Deep Research*) | Busca en cientos de fuentes y entrega un reporte | Un panorama de la literatura (verificando cada fuente) |
| Agente | Usa herramientas: descarga datos, programa, corre código y corrige sus errores | Analizar una base de datos de principio a fin |

Entre más autonomía le das, más cambia tu trabajo: pasas de *ejecutar* a *especificar y revisar*.

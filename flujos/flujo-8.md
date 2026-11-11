---
label: "8. La IA como revisor, no como autor"
order: 92
---
# Flujo 8. La IA como revisor, no como autor

**Para qué sirve:** conseguir crítica honesta de tu trabajo antes de que llegue a tu comité o a una revista, sin que la IA te lo reescriba. **Tiempo:** 30 minutos por revisión. **Herramienta:** cualquier chat gratuito; si tiene modo de razonamiento ("pensar"), actívalo.

## Pregúntale a la IA qué opina de tu trabajo y te va a decir que está excelente

Haz la prueba. Pega tu protocolo y pregunta "¿qué opinas?". Lo más probable es que empiece con algo como "¡Es una propuesta muy interesante y bien estructurada!" y luego te dé tres sugerencias suaves.

No es que tu trabajo sea excelente. Es que la IA está entrenada para agradarte. Las personas que calificaron sus respuestas durante el entrenamiento preferían las que les daban la razón, y el modelo aprendió a darla. Se llama **complacencia** (en inglés, *sycophancy*), y está documentada en todos los modelos grandes: hasta cambian una respuesta correcta por una incorrecta si el usuario insiste (Sharma et al., 2024).

En investigación eso es veneno. Necesitas a alguien que te diga dónde se cae tu argumento antes de que te lo diga tu sinodal.

## Bien pedida, la crítica de la IA se parece a la de un revisor humano

La buena noticia es que, cuando le pides crítica de forma explícita, la IA es sorprendentemente útil.

En un estudio con miles de artículos, los comentarios que generaba GPT-4 coincidían con los de los revisores humanos más o menos tanto como coinciden dos revisores humanos entre sí. Y de 308 investigadores que la probaron con sus propios artículos, más de la mitad dijo que la retroalimentación les había sido útil o muy útil (Liang et al., 2024).

No sustituye a tu asesor. Pero es un primer filtro gratis, disponible a las tres de la mañana, que no se cansa de leer tu capítulo por quinta vez.

## Que la IA revise no es lo mismo que la IA escriba

Hay una tentación natural: si ya encontró los problemas, ¿por qué no dejar que los corrija?

Porque el texto es la parte de la tesis donde ocurre el pensamiento. Escribir te obliga a procesar la información de otra forma. Puedes creer que entiendes un tema, pero no es sino hasta que lo pones por escrito que descubres si es verdad.

Hay evidencia preliminar de lo que pasa cuando delegamos la escritura. En un experimento del MIT, quienes escribieron ensayos con ayuda de ChatGPT mostraron menos actividad cerebral relacionada con el esfuerzo y, minutos después, la mayoría no pudo citar una sola frase de su propio ensayo (Kosmyna et al., 2025). Es un estudio pequeño y todavía sin revisión de pares, pero apunta a algo que cualquier profesor reconoce: si no lo escribiste, no lo aprendiste.

Y hay otro costo. Los profesores ya distinguimos un texto hecho por IA. En cuanto lo notamos, dejamos de leer con atención. ¿Para qué escribir algo que nadie va a leer?

Por eso todos los *prompts* de este flujo terminan igual: **no reescribas nada.**

## Treinta minutos, tres revisores

>>> 1. El revisor adversarial
Para tu protocolo, un capítulo o un artículo antes de enviarlo:

```txt
Actúa como el revisor más exigente de {revista o comité}. Tu trabajo es encontrar las razones para rechazar este trabajo, no para aceptarlo.
1. Enumera los 5 problemas más graves, ordenados por gravedad (datos, método, identificación, argumento, coherencia).
2. Para cada uno, la evidencia en el texto y la pregunta que haría el comité.
3. Señala dónde afirmo más de lo que mi evidencia sostiene.
No me felicites ni reescribas nada.
```

- **"Encontrar las razones para rechazar"** invierte la complacencia: ahora darte gusto es encontrar problemas.
- **"Ordenados por gravedad"** evita que te pierdas en comas mientras se cae tu identificación.
- **"Dónde afirmo más de lo que mi evidencia sostiene"** es la crítica más valiosa en economía: confundir "se mueven juntos" con "uno causa el otro".
- **"No me felicites"** te ahorra el párrafo de cortesía.
>>>

>>> 2. El revisor de estilo que no reescribe
```txt
Revisa mi texto y señala, sin reescribir:
- Oraciones de más de 30 palabras.
- Afirmaciones sin fuente.
- Palabras vagas o infladas.
- Párrafos donde no queda clara la idea principal.
Dame la ubicación y el motivo. Yo hago los cambios.
```

Te da un mapa de dónde trabajar, no un texto nuevo. Los cambios los haces tú, y en el camino aprendes a escribir mejor.
>>>

>>> 3. La prueba a ciegas
Para saber si la IA te está dando la razón por cortesía, no le digas cuál es tu postura:

```txt
Hay dos hipótesis sobre {fenómeno}:
A: {tu hipótesis}
B: {la hipótesis rival}
Dame la evidencia más fuerte a favor y en contra de cada una. No me digas cuál prefieres.
```

Si la evidencia contra tu hipótesis es más fuerte de lo que pensabas, mejor enterarte hoy.
>>>

## "Sí, pero…"

**"¿Y si me equivoco al corregir y la IA lo habría hecho mejor?"** Probablemente lo habría hecho más pulido. Pero sonaría a IA, no sabrías defenderlo y no habrías aprendido nada. Una tesis con tu voz y algunos errores vale más que una tesis impecable que no es tuya.

**"Me hizo una crítica que no comparto."** No tienes que aceptarla. La IA también se equivoca, y tú conoces tu tema mejor. Lo importante es que puedas explicar por qué no aplica; esa explicación es la respuesta que vas a dar en tu examen.

**"¿Puedo pedirle que me corrija solo la ortografía?"** Sí. Corregir ortografía y gramática no cambia tus ideas. Pídele que te señale los errores en una lista para que tú los corrijas, y así no te reescribe el texto de paso.

## Míralo funcionar

Toma el problema del [Flujo 3](flujo-3.md): el gasto del municipio de Chalchihuites en sus fiestas patronales.

Con "¿qué opinas?", la respuesta típica elogia la relevancia local del tema y sugiere "ampliar el marco teórico". No te dice nada que puedas usar.

Con el revisor adversarial, la conversación cambia. Te pregunta cómo vas a saber qué parte del gasto se queda en el municipio si no tienes datos de los proveedores. Te señala que "derrama económica" es un término que suele inflarse si no descuentas lo que la gente habría gastado de todos modos. Y te pregunta contra qué vas a comparar: ¿otro municipio sin fiesta?, ¿otros meses del año?

Cada una de esas preguntas es una pregunta que tu comité te iba a hacer. Ahora tienes tiempo de contestarla.

## Tu turno

!!!success 30 minutos, tus cinco problemas más graves
1. Pega tu protocolo del [Flujo 3](flujo-3.md) con el revisor adversarial.
2. Elige el problema más grave y escribe tú cómo lo resolverías, en un párrafo.
3. Haz la prueba a ciegas con tu hipótesis y la rival más fuerte.

Si la IA no encontró nada grave, pídele que lo intente otra vez "como si tu reputación dependiera de encontrar un error". Siempre hay algo.
!!!

## Referencias de este flujo

- Kosmyna, N., Hauptmann, E., Yuan, Y. T., et al. (2025). Your brain on ChatGPT: Accumulation of cognitive debt when using an AI assistant for essay writing task. *arXiv*, 2506.08872.
- Liang, W., Zhang, Y., Cao, H., et al. (2024). Can large language models provide useful feedback on research papers? A large-scale empirical analysis. *NEJM AI*, 1(8).
- Sharma, M., Tong, M., Korbak, T., et al. (2024). Towards understanding sycophancy in language models. *International Conference on Learning Representations (ICLR)*.

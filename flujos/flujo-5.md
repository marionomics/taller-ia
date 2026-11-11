# Flujo 5. Diseño de instrumento

> *¡Datos! ¡Datos! ¡Datos! No puedo hacer ladrillos sin arcilla.* — Sherlock Holmes

**Para qué sirve:** diseñar un cuestionario que mida lo que dices que mide, desde la teoría hasta las preguntas, y probarlo antes de salir a campo. **Tiempo:** 1 hora para el primer borrador. **Herramienta:** cualquier chat gratuito.

## Si tus datos son basura, tu tesis también

Lo que está en el centro de tu investigación es la solidez de tus argumentos. Pero esos argumentos se apoyan en datos. En inglés lo dicen mejor: *garbage in, garbage out*. Si entra basura, sale basura, por más sofisticado que sea tu modelo.

Me ha pasado que me invitan a colaborar en una investigación y he tenido que decir que no. No por el tema, sino porque no sé cómo se obtuvieron los datos, nadie lo documentó y no tengo forma de saber si los resultados son válidos.

Cuando tú levantas tus propios datos, ese riesgo está en tus manos. Y el lugar donde más se echa a perder es en las preguntas.

## Cambiar una palabra cambia la respuesta

En 1940, un investigador hizo la misma pregunta a dos grupos con una sola palabra distinta. ¿Debería Estados Unidos *permitir* discursos públicos en contra de la democracia? El 62 % dijo que no se debían permitir. ¿Debería *prohibirlos*? Solo el 46 % dijo que sí se debían prohibir (Rugg, 1941). Lógicamente es lo mismo, pero la gente no responde como lógico.

Y hay un problema más grande: la gente responde lo que se ve bien. Si preguntas "¿lee usted con frecuencia?" o "¿su empresa innova?", vas a obtener más "sí" de los que hay en la realidad. Se llama **sesgo de deseabilidad social**, y está documentado de sobra en encuestas (Tourangeau y Yan, 2007).

Por eso no puedes preguntarle a un empresario "¿se considera usted innovador?". Diez personas te darían diez definiciones distintas, todas favorables.

## Párate en hombros de gigantes; la IA te ayuda con los ladrillos

La forma correcta de medir un concepto abstracto es descomponerlo. Vas a la literatura (el [Flujo 4](flujo-4.md)) y de ahí sacas cómo se ha definido y medido. Un concepto se divide en **subíndices**, cada subíndice en **variables** y cada variable en **indicadores**. Cada indicador se convierte en una pregunta.

Así lo hicimos en un estudio sobre los determinantes de la innovación en las micro y pequeñas empresas del Valle de México, en el que participé como autor. Antes de que existiera ChatGPT, diseñar los reactivos nos tomó semanas.

Hoy el borrador toma un minuto. La estructura (subíndices y variables) la pones tú, desde la teoría. Los reactivos, que son el trabajo pesado y repetitivo, se los pides a la IA con reglas claras.

## La IA escribe preguntas que suenan bien y miden mal

Si le pides "hazme un cuestionario sobre innovación", te va a dar preguntas como "¿Considera que su empresa tiene una cultura de innovación?". Suenan profesionales. Son inútiles: invitan a la respuesta deseable y cada quien las interpreta distinto.

Los otros tropiezos comunes:

- **Preguntar por intenciones o sentimientos** ("¿planea invertir en tecnología?"). Mide buenos deseos, no conducta.
- **Meter dos cosas en una pregunta** ("¿su empresa capacita y motiva a sus empleados?"). Si contestan "de acuerdo", no sabes a cuál de las dos.
- **Creer que el borrador es el instrumento.** La validación (expertos, prueba piloto, confiabilidad) sigue siendo tuya.

## Una hora, cuatro pasos

>>> 1. Dibuja tu índice desde la teoría
Del centro hacia afuera: concepto → subíndices → variables. Sácalo de la literatura o de instrumentos que ya existen. Por ejemplo: Innovación → Organización → Visión de futuro.
>>>

>>> 2. Pide los reactivos con reglas estrictas
```txt
Eres un investigador con amplia experiencia en métodos cuantitativos y diseño de instrumentos.
El indicador mide {innovación en pequeñas empresas}. Te pasaré subíndices y variables.
Para cada variable genera 2 o 3 indicadores y una sentencia Likert por indicador.
Las sentencias deben ser concretas y ancladas en hechos verificables (presupuestos, tiempos, acciones), evitar el sesgo de deseabilidad social y no requerir interpretación subjetiva. Nada de intenciones futuras ni sentimientos abstractos.
Ejemplo (subíndice "Organización", variable "Visión de futuro"): "Estamos desarrollando hoy productos que sabemos que el cliente necesitará, aunque hoy no los pida".
Dime cuando estés listo.
```

- **"Hechos verificables"** es tu defensa contra la deseabilidad social: es más difícil exagerar un presupuesto que una opinión.
- **"Nada de intenciones futuras"** saca de la mesa los buenos deseos.
- **El ejemplo** vale más que cualquier instrucción. Le muestra el nivel de concreción que esperas.
- **Escala Likert:** las respuestas van de "totalmente en desacuerdo" a "totalmente de acuerdo". Te permite medir sin preguntar directamente "¿es usted innovador?".
>>>

>>> 3. Ponlo a prueba con un encuestado difícil
Antes de molestar a personas reales, usa a la IA para encontrar los problemas obvios:

```txt
Ahora actúa como {dueño de una tienda de abarrotes en Gómez Palacio, con secundaria terminada}.
Lee cada pregunta del cuestionario y dime:
- cuáles no entiendes o entenderías de otra forma,
- cuáles contestarías "de acuerdo" solo para quedar bien,
- cuáles tienen dos preguntas en una.
```

Esto **no** sustituye la prueba piloto. Cuando se ha probado a la IA como "encuestado sintético", sus respuestas se alejan bastante de las de personas reales (ver el recuadro del [Flujo 6](flujo-6.md)). Sirve para limpiar el borrador, nunca como datos.
>>>

>>> 4. Valida con humanos
Pásalo a dos o tres expertos en el tema, haz una prueba piloto con personas parecidas a tu muestra y revisa la confiabilidad de tus escalas (por ejemplo, con el alfa de Cronbach). Si quieres convertir tu cuestionario en un formulario en línea sin capturar todo a mano, ve al [Flujo 7](flujo-7.md).
>>>

## "Sí, pero…"

**"¿No hay un instrumento que ya exista?"** Muchas veces sí, y es mejor usarlo: ya está validado y puedes comparar tus resultados. Búscalo primero en la literatura. Diseña uno propio solo si no existe o no se adapta a tu contexto.

**"¿Cuántas preguntas por variable?"** Al menos dos. Con una sola no puedes saber si la pregunta mide lo que crees o si la gente la entendió mal.

**"¿Y si uso datos que ya existen, como los de INEGI?"** Entonces no diseñas instrumento, pero tienes la misma obligación: conocer cómo se levantaron como si lo hubieras hecho tú. Eso está en el paso 0 del [Flujo 6](flujo-6.md).

## Míralo funcionar

Con el ejemplo de innovación: subíndice "Organización", variable "Visión de futuro".

Lo que la IA suele proponer sin reglas: *"En mi empresa se valora la innovación."* Todos van a contestar que sí.

Con el *prompt* del paso 2 salen cosas como: *"En el último año destinamos parte del presupuesto a probar un producto o servicio nuevo."* Eso es verificable. Un empresario puede exagerar un poco, pero no puede inventar un presupuesto que no tiene sin darse cuenta de que miente.

Y en la prueba con el encuestado difícil, la IA señala que "producto o servicio nuevo" es ambiguo: ¿nuevo para el mercado o nuevo para la tienda? Ese es justo el tipo de detalle que un piloto te habría dicho, pero ya lo tienes antes de imprimir.

## Tu turno

!!!success 1 hora, una variable bien medida
1. Elige un concepto de tu tesis y baja hasta una sola variable.
2. Genera sus reactivos con el *prompt* del paso 2.
3. Pásalos por el encuestado difícil del paso 3.
4. Marca cuáles sobreviven. Esos son los que llevas al piloto.
!!!

## Referencias de este flujo

- Rugg, D. (1941). Experiments in wording questions: II. *Public Opinion Quarterly*, 5(1), 91–92.
- Tourangeau, R. y Yan, T. (2007). Sensitive questions in surveys. *Psychological Bulletin*, 133(5), 859–883.

# Flujo 7. Artefactos: formularios, tableros y laboratorios

**Para qué sirve:** construir pequeñas herramientas para tu investigación (una calculadora, un formulario, un tablero de resultados) sin saber programar, y saber revisarlas antes de confiar en ellas. **Tiempo:** 30 minutos para tu primera herramienta. **Herramienta:** los **artefactos** de Claude o el **Canvas** de Gemini y ChatGPT; los tres funcionan en la versión gratuita.

## Tu investigación necesita herramientas que nadie te va a hacer

Piensa en todo lo que una investigación necesita además del texto: un formulario para levantar tu encuesta, una calculadora para decidir el tamaño de tu muestra, un tablero para ver cómo van llegando las respuestas, un simulador para explicarle tu modelo a tu comité.

Hasta hace muy poco tenías tres opciones: aprender a programar, pagarle a alguien o hacerlo todo a mano en Excel. La mayoría escogía la tercera, y así nacían las hojas de cálculo frágiles que vimos en el [Flujo 6](flujo-6.md).

## Ahora describes la herramienta y la IA la construye

La IA ya no solo escribe texto: construye cosas que funcionan. Un **artefacto** (así le llama Claude; en Gemini y ChatGPT se llama Canvas) es una ventana al lado del chat donde la IA escribe un programa pequeño y lo puedes usar al momento: una página con botones, gráficas y cálculos. Le pides cambios en el chat y se actualiza.

La ganancia es real. En un experimento con programadores, quienes usaron un asistente de IA terminaron la misma tarea 56 % más rápido que quienes no lo usaron (Peng et al., 2023). Para alguien que no programa, la diferencia es todavía mayor: es pasar de "no puedo" a "lo tengo en media hora".

Algunas cosas que he hecho así:

- **Formularios automáticos.** Un script de Google Apps Script que crea el Google Form a partir de mis reactivos, y otro que envía la encuesta por correo a una lista. Así levanté el seguimiento a egresados de la FECA.
- **Tableros de resultados.** Una página que lee las respuestas de un instrumento y las muestra en gráficas desde el primer día del levantamiento.
- **Laboratorios para clase.** Páginas para que mis alumnos de Investigación de Operaciones experimenten con el problema del agente viajero o la ruta más corta.

## Una herramienta bonita no es una herramienta correcta

Este es el riesgo: la IA hace herramientas que **se ven** profesionales. Botones, colores, gráficas animadas. Y nuestra cabeza confunde "se ve bien" con "está bien".

Una calculadora con una fórmula equivocada da números equivocados con la misma seguridad que una correcta. Por eso la regla de este flujo es: **antes de usarla, pruébala con un caso del que ya sepas la respuesta.**

Otros dos cuidados:

- **No subas datos personales** de tus encuestados a una herramienta que se puede compartir con un enlace.
- **Documenta qué hace.** Si presentas resultados que salieron de un tablero, tienes que poder explicar cada número. Si no, no pasa la prueba de la revelación (ver [Qué es recomendable y qué no](../que-es-recomendable.md)).

## Treinta minutos, cuatro pasos

>>> 1. Describe la herramienta como si se la pidieras a un programador
Qué entra, qué sale, qué cálculo hace y para quién es. Entre más claro, menos vueltas.
>>>

>>> 2. Pídela en modo artefacto o Canvas
```txt
Crea una herramienta interactiva (artefacto) para {propósito}.
Entradas: {qué escribe o elige el usuario}.
Salidas: {qué muestra: números, tabla, gráfica}.
Cálculo: {fórmula o regla; si no la sabes, pídele que la explique antes de programarla}.
Debajo del resultado, muestra la fórmula que usaste y los valores que sustituiste.
Interfaz en español, sencilla y legible en celular.
```

"Muestra la fórmula y los valores" convierte una caja negra en algo que puedes revisar.
>>>

>>> 3. Pruébala con un caso conocido
Busca un ejemplo resuelto en un libro, en un artículo o hazlo a mano. Si la herramienta no da lo mismo, díselo a la IA con el caso concreto: "con estos valores debería dar X y me da Y".
>>>

>>> 4. Ajusta y guárdala
Pide cambios en lenguaje normal ("agrega un campo para…", "pon la gráfica en barras"). Cuando funcione, puedes publicarla y compartir el enlace, o descargar el archivo.
>>>

## "Sí, pero…"

**"¿Necesito saber programar?"** No para construirla. Sí necesitas saber qué debería calcular, igual que en el [Flujo 6](flujo-6.md). La IA programa; tú verificas.

**"¿Puedo usar esto para mi encuesta real?"** Para crear el formulario, sí: pídele un script de Google Apps Script que genere el Google Form con tus reactivos. Te dice paso a paso dónde pegarlo. Para guardar respuestas de personas reales, usa una herramienta establecida como Google Forms, no una página improvisada.

**"¿Y si quiero algo más grande, como una plataforma?"** Ahí ya entras al terreno de los agentes y del desarrollo de software. Es posible, pero es otro nivel; lo verás al final de esta página.

## Míralo funcionar: una calculadora de tamaño de muestra

Necesitas saber cuántas personas encuestar. La fórmula clásica para estimar una proporción es:

$$n_0 = \frac{z^2 \, p(1-p)}{e^2}$$

donde $z$ es 1.96 para un 95 % de confianza, $p$ es la proporción esperada (0.5 si no tienes idea, porque es el caso más exigente) y $e$ es el margen de error. Si tu población es pequeña, se corrige con $n = n_0 / \left(1 + \frac{n_0 - 1}{N}\right)$, donde $N$ es el tamaño de la población.

Le pido a la IA una calculadora con esas entradas, usando el *prompt* del paso 2. Antes de usarla, la pruebo con un caso que sé de memoria: con 95 % de confianza, $p = 0.5$ y 5 % de error, la respuesta tiene que ser **385** (384.16, redondeado hacia arriba). Y si la población es de 2,000 personas, tiene que dar **323**.

Si da esos números, confío en ella. Si no, ya sé que algo está mal antes de salir a campo con una muestra equivocada.

## Tu turno

!!!success 30 minutos, tu primera herramienta
1. Abre Claude (artefactos) o Gemini (Canvas) en su versión gratuita.
2. Pide la calculadora de tamaño de muestra con el *prompt* del paso 2.
3. Pruébala: ¿da 385 sin corrección y 323 con una población de 2,000?
4. Cámbiale los valores a los de tu investigación y anota tu tamaño de muestra.

Bonus: pídele que agregue una gráfica de cómo cambia la muestra según el margen de error. Vas a ver por qué pasar de 5 % a 3 % de error casi triplica las encuestas.
!!!

!!!primary Cuando quieras construir en serio
Los artefactos son el primer paso. Con agentes como **Claude Code** puedes construir tableros que se conectan a tus datos, automatizar el envío de encuestas o armar el sitio de tu proyecto. En mi comunidad **Economista Full Stack** comparto los scripts y plantillas que uso, y en las sesiones semanales puedes traer lo que estés construyendo. Tienes **7 días gratis** para probarla y cancelas cuando quieras.

[!button variant="primary" text="Probar 7 días gratis"](https://www.skool.com/economista-full-stack-6510/about)
!!!

## Referencias de este flujo

- Peng, S., Kalliamvakou, E., Cihon, P. y Demirer, M. (2023). The impact of AI on developer productivity: Evidence from GitHub Copilot. *arXiv*, 2302.06590.

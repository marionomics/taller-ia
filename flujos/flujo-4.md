---
label: "4. Bibliografía y marco teórico a prueba de balas"
order: 96
---
# Flujo 4. Bibliografía y marco teórico a prueba de balas

> *Los hombres prácticos, que se creen exentos de cualquier influencia intelectual, son usualmente esclavos de algún economista difunto.* — John Maynard Keynes

**Para qué sirve:** encontrar la literatura que sostiene (y la que contradice) tu hipótesis, verificar que existe y armar con ella el esqueleto de tu marco teórico. **Tiempo:** 1 hora para la búsqueda; la lectura es aparte. **Herramienta:** el modo de investigación profunda de Gemini o ChatGPT (ambos tienen algunos usos gratis al mes), Google Scholar y NotebookLM.

## Imagina que es 1987 y necesitas un artículo

Estás leyendo un *paper* y ves citado un estudio que tiene justo lo que necesitas. ¿Cómo lo consigues? Le escribes una carta al autor, o le llamas por teléfono. Días después, si tienes suerte, te llega una copia por fax.

Te cuento esto porque el sistema de citas es mucho más viejo que las computadoras, y descansa en una promesa: **cuando citas algo, es porque lo leíste.** La cita no es un adorno; es la forma en que los investigadores conectan su trabajo y dicen "esto es lo que vale la pena revisar".

Esa promesa ya se rompía antes de la IA. Dos físicos estudiaron cómo se copian los errores de imprenta en las referencias de un artículo famoso: el mismo error aparecía una y otra vez, lo que solo pasa si copias la cita de otro sin abrir el original. Su estimación fue que cerca del 80 % de quienes citaban no habían leído el artículo (Simkin y Roychowdhury, 2003).

## La IA no lee lo que cita: predice lo que suena a cita

Con la IA el problema se vuelve industrial. Como vimos en [Cómo funciona la IA](../como-funciona-la-ia.md), el modelo no consulta una biblioteca: genera lo que suena más probable. Y una referencia que suena muy real es fácil de generar.

Cuando lo midieron, el 55 % de las referencias que daba GPT-3.5 eran inventadas, y el 18 % de las de GPT-4; además, muchas de las reales tenían errores en autores, años o páginas (Walters y Wilder, 2023). Los modelos de hoy inventan menos, sobre todo cuando buscan en internet, pero no llegan a cero.

Yo hice un experimento sencillo: le pedí 10 artículos sobre un tema. Solo 2 tenían el enlace correcto. Ocho artículos sí existían, pero en la mitad de ellos las conclusiones que me daba eran inventadas.

Citar algo que no existe, o que no dice lo que tú dices, es de los peores pecados de una tesis, con o sin IA. No solo te delata: deja claro que no abriste tus fuentes.

## "Dame bibliografía sobre mi tema" te da, en el mejor caso, una lista genérica

En el peor caso, inventada.

Para pedir buenas referencias necesitas tres cosas: el objetivo de tu investigación, tu argumento y sus posibles contraargumentos. Por eso este flujo va después del [protocolo](flujo-3.md). Sin protocolo, la IA no sabe qué buscar.

También necesitas saber que no todas las fuentes valen lo mismo. Puedes citar un video de YouTube o una revelación que tuviste en un sueño (hay un filósofo que lo hizo en una nota al pie). Pero un experimento vale más que una encuesta autorreportada, y un artículo arbitrado más que un blog. Si no se lo pides, la IA mezcla todo.

## Una hora, cuatro pasos

>>> 1. Pide la búsqueda con investigación profunda
Usa el modo de **investigación profunda** (*Deep Research*): la IA hace decenas de búsquedas y te entrega un reporte con fuentes. Es como mandar a tu becario a pasarse la noche buscando, sin tener que invitarle el café. Pega tu protocolo después de este *prompt*:

```txt
Eres mi asistente de investigación. Te pasaré mi protocolo.
1. Identifica los temas principales de los que necesito referencias.
2. Incluye referencias que apoyen mi hipótesis y otras que la contradigan.
3. Organiza en una tabla: cita APA, DOI o enlace, diseño del estudio, tamaño de muestra, resultado principal.
4. Ordena por calidad metodológica (experimentos y cuasiexperimentos primero). Prioriza revistas arbitradas.
5. Marca explícitamente cualquier referencia que no hayas podido abrir.
Lista negra (no incluyas): {referencias que ya tienes o que descartaste}
```

- **"Que la contradigan"** combate la tendencia de la IA a darte la razón. Un marco teórico solo con evidencia a favor no resiste la primera pregunta de tu comité.
- **Diseño y tamaño de muestra** te dejan ver de un vistazo qué tan sólido es cada estudio.
- **"Marca lo que no pudiste abrir"** es tu primera alarma de referencias sospechosas.
- **La lista negra** evita que te repita lo que ya tienes.
>>>

>>> 2. Verifica cada referencia (no te saltes este paso)
- [ ] La referencia existe: búscala por título o DOI en Google Scholar, no con el enlace que te dio.
- [ ] La abriste y leíste al menos el resumen y la sección que vas a citar.
- [ ] Dice lo que tú dices que dice.
- [ ] Autor, año, revista y páginas coinciden.

Para leer más rápido, sube los artículos a **NotebookLM** (gratis con una cuenta de Google). Responde con base solo en los documentos que le das, y puedes preguntarle cosas como si hablaras con el autor.
>>>

>>> 3. Arma el esqueleto del marco teórico
El error más común en el marco teórico es meter un montón de citas más o menos relacionadas. Una vez un amigo me contó que una profesora le dijo que se trataba de "poner una cita en cada párrafo". Me quería sacar los ojos.

El marco teórico existe para **sostener tu hipótesis**. Para eso, de cada concepto clave necesitas saber tres cosas: **qué significa**, **cómo lo sabemos** (la evidencia) y **por qué importa** para tu pregunta.

```txt
Para el tema que te daré, identifica las teorías clave con enfoque en {economía}. De cada una dime: qué significa, cómo lo sabemos (evidencia) y por qué importa para mi pregunta. Incluye teorías alternativas y contraejemplos. Dame una tabla con referencias en APA.
```

"Con enfoque en {economía}" evita que se vaya por las ramas. Si investigas un impuesto a los refrescos y no le dices el enfoque, puede terminar explicándote el metabolismo de la glucosa.
>>>

>>> 4. Revisa que la tabla tenga lo que tú esperabas
Antes de leer la tabla, anota una teoría que estás seguro de que debería aparecer. Si no aparece, la IA no entendió tu tema: dale más contexto. Si aparece, vas bien. Después usa la tabla como **mapa de lectura**, no como texto para tu tesis.
>>>

## "Sí, pero…"

**"Verificar cada referencia me va a tomar horas."** Sí. Menos de lo que te tomaría explicarle a tu comité por qué citaste un artículo que no existe. Y lo que no verificas, no lo citas.

**"Mi tema es muy local; casi no hay literatura."** Busca en dos niveles: el fenómeno en general (en cualquier país) y tu contexto específico (aunque sean reportes de gobierno o tesis). Pídele a la IA las dos cosas por separado.

**"¿Puedo pedirle que me haga la cita en APA?"** Sí, y es de los mejores usos. Pásale el enlace o los datos del artículo que tú ya encontraste y leíste, y pídele: "Escribe la cita en formato APA de esta fuente". Así trabajo yo casi siempre: guardo lo que voy leyendo y dejo que la IA haga el formato.

## Míralo funcionar

Supón que tu tema es el efecto del impuesto a las bebidas azucaradas en el consumo y la diabetes. Antes de correr el *prompt* del paso 3, anoto lo que espero ver: la teoría del **impuesto pigouviano** (un impuesto que hace que quien genera un costo para otros lo pague).

Cuando lo hice, el impuesto pigouviano apareció en la tabla sin que yo lo mencionara. Eso me dijo que la IA había entendido el tema y el enfoque.

Una buena tabla para este tema se organiza en tres bloques: los impuestos pigouvianos y las externalidades; la evidencia sobre cómo responde el consumo a los precios (la *elasticidad*); y la literatura médica sobre azúcar y diabetes. Y a veces trae algo que no habías pensado, como estudios sobre si el impuesto se traslada completo al precio o si las empresas absorben una parte. Si esa pregunta intermedia es clave para tu hipótesis, ya sabes qué leer primero.

## Tu turno

!!!success 1 hora, tu propia tasa de errores
1. Corre el *prompt* del paso 1 con tu protocolo.
2. Elige 5 referencias de la tabla y verifícalas con la checklist del paso 2.
3. Cuenta cuántas pasaron las cuatro casillas.

Esa es tu tasa de errores con esa herramienta y ese tema. Te va a quitar las ganas de copiar referencias sin abrirlas.
!!!

## Referencias de este flujo

- Simkin, M. V. y Roychowdhury, V. P. (2003). Read before you cite! *Complex Systems*, 14(3), 269–274.
- Walters, W. H. y Wilder, E. I. (2023). Fabrication and errors in the bibliographic citations generated by ChatGPT. *Scientific Reports*, 13, 14045.

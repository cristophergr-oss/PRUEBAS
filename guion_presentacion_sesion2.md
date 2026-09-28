# Guion de exposición (90 segundos) — Sesión 2

**Tema del equipo:** Análisis de sentimiento (PLN / IA).
**Problema central (mapa mental):** ¿qué método clasifica mejor las mismas reseñas en español? Necesitamos una comparación fiable.

**Reparto sugerido:** 3 voces (A, B, C). Si son 2 o 4 integrantes, redistribuyan los bloques.
**Ritmo:** unas 210 palabras habladas. Ensayar con cronómetro.

---

## Bloque 1 — Contexto, causas y problema central (0:00 – 0:25) · Voz A

> Buenos días. Somos el equipo [nombre]. Nuestro tema es el análisis de sentimiento: clasificar
> opiniones en reseñas como positivas, negativas o neutras. La causa del problema es que el
> lenguaje de las reseñas es ambiguo y variado, y cada método lo procesa distinto.
> Nuestro problema central: **¿qué método clasifica mejor las mismas reseñas en español?**
> Necesitamos una comparación fiable, porque una mala elección produce clasificaciones poco fiables.

## Bloque 2 — Pregunta de investigación y evidencia (0:25 – 1:05) · Voz B

> La pregunta de investigación queda así:
> **¿En qué medida un modelo preentrenado tipo BERT en español supera a métodos tradicionales,
> como SVM y Naive Bayes, al clasificar la polaridad de reseñas en español, evaluados sobre los
> mismos datos?**
>
> La evidencia que permitiría responderla: un conjunto de **reseñas etiquetadas, el mismo para
> todos los métodos**, con el mismo preprocesamiento. Comparamos **F1 macro**, analizamos los
> **errores** de cada modelo con su matriz de confusión y medimos el **tiempo de ejecución**.
> Si la diferencia de F1 se mantiene en todas las particiones de validación cruzada, la pregunta
> queda respondida con datos y no con opinión.

## Bloque 3 — Cambio de decisión (1:05 – 1:25) · Voz C

> La decisión que cambió: partimos del tema amplio "análisis de sentimiento", que abarcaba
> emociones, tuits, tickets de soporte y llamadas. Lo acotamos a **comparar dos enfoques,
> tradicional y preentrenado, sobre reseñas en español**, porque es donde tenemos fuentes
> revisadas y datos etiquetados accesibles.

## Cierre (1:25 – 1:30) · Voz C

> Con la pregunta delimitada, hoy toca convertirla en acciones concretas y verificables. Gracias.

---

## Posibles preguntas del grupo o del docente (respuesta en una frase)

- **¿Por qué F1 macro y no accuracy?**
  Porque las clases suelen estar desbalanceadas y el accuracy esconde fallos en la clase minoritaria.
- **¿De dónde salen las reseñas?**
  De un corpus público etiquetado en español, o de reseñas recogidas y etiquetadas por el equipo con acuerdo entre anotadores.
- **¿Por qué medir tiempo de ejecución?**
  Porque si BERT gana por poco pero cuesta diez veces más, la elección práctica cambia.
- **¿Y la ironía o el sarcasmo?**
  Es un reto conocido; lo registramos en el análisis de errores en lugar de prometer resolverlo.
- **¿Terminaron la revisión bibliográfica?**
  No del todo: NotebookLM no pudo leer varios artículos y los estamos revisando a mano esta semana.

---

## Versión de emergencia (45 segundos, si van tarde)

> Tema: análisis de sentimiento en reseñas. Problema: el lenguaje es ambiguo y cada método lo
> procesa distinto, así que una mala elección da clasificaciones poco fiables. Pregunta: ¿en qué
> medida BERT en español supera a SVM y Naive Bayes al clasificar reseñas en español sobre los
> mismos datos? Evidencia: reseñas etiquetadas, F1 macro, análisis de errores y tiempo de
> ejecución. Decisión que cambió: del tema amplio a comparar dos enfoques en reseñas en español.
> Gracias.

---

## Anexo — Cadena del documento (Tema → Problema → Pregunta → Objetivos)

**Tema.** Análisis de sentimiento con procesamiento de lenguaje natural e IA.

**Problema.** Las reseñas en español usan un lenguaje ambiguo y variado; los distintos métodos de
clasificación lo procesan de forma diferente y no existe una comparación fiable sobre los mismos
datos, por lo que una mala elección de método produce clasificaciones poco fiables.

**Pregunta de investigación.** ¿En qué medida un modelo preentrenado tipo BERT en español supera
a métodos tradicionales (SVM y Naive Bayes) al clasificar la polaridad de reseñas en español,
evaluados sobre los mismos datos?

**Objetivo general.** Comparar de forma controlada un enfoque tradicional y un enfoque
preentrenado para la clasificación de polaridad de reseñas en español, sobre el mismo conjunto
de datos, en términos de F1, errores y tiempo de ejecución.

**Objetivos específicos.**
1. Obtener un conjunto de reseñas en español etiquetadas por polaridad y definir un preprocesamiento común.
2. Entrenar y evaluar una línea base tradicional con SVM y Naive Bayes sobre TF-IDF.
3. Ajustar y evaluar un modelo preentrenado tipo BERT en español sobre los mismos datos.
4. Comparar ambos enfoques con F1 macro y validación cruzada, y analizar sus errores con matrices de confusión.
5. Medir y comparar el tiempo de ejecución de cada enfoque para valorar su viabilidad práctica.

---

## Fuentes revisadas

- Análisis de sentimiento de tuits sobre la COP9: comparación de modelos preentrenados y técnicas tradicionales (PMC).
- Transfer learning para clasificación de sentimientos con BERT (PMC).
- Análisis de sentimientos en contexto multilingüe: machine learning vs. modelos híbridos de deep learning (PMC).
- Predicción de sentimiento con transformers y modelos previos, distintos embeddings, reseñas de Amazon (PMC).
- SEDICI UNLP: análisis de opiniones en español con técnicas de machine learning.
- SciELO Chile: clasificación de polaridad en textos en español.
- Revista Espacios: opiniones sobre #BlackFriday en Twitter.
- Redalyc: análisis de sentimientos de críticas gastronómicas con ontologías.
- Cuaderno y mapa mental del equipo en NotebookLM.

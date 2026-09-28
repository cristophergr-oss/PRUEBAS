# Guion de exposición (90 segundos) — Sesión 2

**Tema del equipo:** Análisis de sentimientos en textos en español con machine learning:
modelos preentrenados (BERT / transformers) frente a técnicas tradicionales (SVM, Naive Bayes, ontologías).

**Reparto sugerido:** 3 voces (A, B, C). Si son 2 o 4 integrantes, redistribuyan los bloques.
**Ritmo:** unas 210 palabras habladas. Ensayar con cronómetro.

---

## Bloque 1 — Mapa de problema y pregunta (0:00 – 0:20) · Voz A

> Buenos días. Somos el equipo [nombre]. En la sesión 1 nuestro mapa de problema partió de un hecho:
> cada día se publican millones de opiniones en español en redes sociales y sitios de reseñas,
> pero son texto no estructurado y la mayoría de modelos y datasets de análisis de sentimientos
> están pensados para el inglés. El problema que delimitamos es: **¿qué técnica clasifica mejor
> la polaridad de opiniones en español?**

## Bloque 2 — Pregunta de investigación y evidencia (0:20 – 1:05) · Voz B

> Nuestra pregunta de investigación queda así:
> **¿En qué medida un modelo preentrenado tipo BERT en español supera a técnicas tradicionales,
> como SVM y Naive Bayes con TF-IDF, al clasificar la polaridad de tuits en español,
> medido con F1 macro sobre un mismo corpus?**
>
> La evidencia que permitiría responderla es una **comparación controlada**: los mismos tuits
> etiquetados como positivo, negativo o neutro, el mismo preprocesamiento, y cada modelo evaluado
> con validación cruzada. El resultado se presenta en una **tabla de F1 macro, precisión y recall**,
> más la **matriz de confusión** de cada modelo. Si la diferencia de F1 es consistente en todas
> las particiones, la pregunta queda respondida con datos y no con opinión.

## Bloque 3 — Decisión que cambió (1:05 – 1:25) · Voz C

> Una decisión que cambió durante el trabajo: al principio queríamos mezclar tuits, reseñas de
> productos y críticas gastronómicas. Al revisar las fuentes vimos que el dominio del texto
> altera el rendimiento de los modelos, así que **acotamos el estudio a un solo dominio, tuits**,
> para que la comparación sea justa y viable en el tiempo del curso.

## Cierre (1:25 – 1:30) · Voz C

> Con la pregunta delimitada, el siguiente paso es convertirla en acciones concretas y verificables.
> Gracias.

---

## Posibles preguntas del grupo o del docente (respuesta en una frase)

- **¿Por qué F1 macro y no accuracy?**
  Porque las clases suelen estar desbalanceadas y el accuracy esconde que el modelo falle en la clase minoritaria.
- **¿De dónde saldrá el corpus de tuits?**
  De un corpus público etiquetado en español (por ejemplo TASS) o de tuits recolectados con un hashtag y etiquetados por el equipo con acuerdo entre anotadores.
- **¿Por qué BERT en español y no BERT multilingüe?**
  Porque las fuentes muestran que un modelo preentrenado en el idioma objetivo captura mejor el léxico y la ironía locales.
- **¿Es viable entrenar BERT con sus recursos?**
  Sí, solo hacemos fine-tuning sobre un modelo ya preentrenado, que corre en una GPU gratuita tipo Colab.
- **¿Qué pasa si los modelos tradicionales ganan?**
  También es un resultado válido: significaría que para este dominio el costo computacional de BERT no se justifica.

---

## Versión de emergencia (45 segundos, si van tarde)

> Nuestro problema: hay millones de opiniones en español sin estructurar y la mayoría de herramientas
> están hechas para inglés. Pregunta: ¿en qué medida BERT en español supera a SVM y Naive Bayes al
> clasificar la polaridad de tuits, medido con F1 macro sobre el mismo corpus? Evidencia: tabla
> comparativa de F1, precisión y recall con validación cruzada, más matrices de confusión.
> Decisión que cambió: pasamos de mezclar reseñas, críticas y tuits a un solo dominio, tuits,
> para que la comparación sea justa y viable. Gracias.

---

## Fuentes que sostienen el guion

- Análisis de sentimiento de tuits sobre la COP9: comparación de modelos preentrenados y técnicas tradicionales (PMC).
- Transfer learning para clasificación de sentimientos con BERT (PMC).
- Análisis de sentimientos en contexto multilingüe: machine learning vs. modelos híbridos de deep learning (PMC).
- Predicción de sentimiento con transformers y modelos previos, distintos embeddings, reseñas de Amazon (PMC).
- SEDICI UNLP: análisis de opiniones en español con técnicas de machine learning.
- SciELO Chile: clasificación de polaridad en textos en español.
- Revista Espacios: opiniones sobre #BlackFriday en Twitter.
- Redalyc: análisis de sentimientos de críticas gastronómicas con ontologías.

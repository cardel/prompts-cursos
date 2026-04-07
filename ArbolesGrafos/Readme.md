# Tutores Virtuales — Árboles y Grafos

**Pontificia Universidad Javeriana Cali**
Curso: Árboles y Grafos — Ingeniería de Sistemas / Ciencias de la Computación
Semestre: 4to

---

## Descripción

Este repositorio contiene un conjunto de **9 prompts pedagógicos** diseñados como tutores virtuales de apoyo al aprendizaje para estudiantes del curso de Árboles y Grafos. Cada prompt está pensado para ser copiado y pegado directamente en una conversación con un LLM (ChatGPT, Claude, Gemini, etc.), donde el estudiante recibirá acompañamiento socrático estructurado.

**Principio fundamental:** Estos tutores son herramientas de APOYO. El profesor del curso lidera el proceso académico, acompaña el avance, toma las decisiones y evalúa formalmente. Los tutores NUNCA reemplazan al profesor y NUNCA entregan soluciones completas.

---

## Estructura del Curso

El curso se organiza en **3 temáticas** alineadas con el cronograma y el texto guía CLRS (*Introduction to Algorithms*, Cormen et al.):

| Temática | Contenido | Referencia CLRS |
|---|---|---|
| **T1 — Fundamentos y Grafos Básicos** | Notación asintótica, invariantes de ciclo, demostraciones de correctitud, Divide y Conquista, búsqueda binaria, bisección, definiciones formales de grafos, representaciones, DFS, BFS, grafos implícitos | Caps. 2-4, 22.1-22.3 |
| **T2 — Grafos Avanzados** | Orden topológico, componentes conexos, SCC (Kosaraju), puntos de articulación, puentes, biconexos, caminos más cortos (BFS, Bellman-Ford, Dijkstra, Floyd-Warshall) | Caps. 22.4-22.5, 24, 25 |
| **T3 — Árboles, Estructuras Jerárquicas y Cadenas** | Árboles (diámetro, radio, centro), Segment Trees, Union-Find, Fenwick Trees, MST (Kruskal, Prim), arreglos de sufijos, soporte al Proyecto Final | Caps. B.5, 21, 23 + Halim |

---

## Las 3 Categorías de Tutores

Cada temática tiene **3 tutores** que trabajan en paralelo, cada uno con un enfoque pedagógico distinto:

### Euler — Tutor Conceptual

**Enfoque:** Conductista con refuerzo progresivo.
**Propósito:** Dominio formal de definiciones, teoremas, demostraciones y propiedades matemáticas. Trabaja con notación formal (cuantificadores, conjuntos, invariantes) sin implementación en código.
**Cuándo usarlo:** Cuando necesitas entender un concepto, razonar formalmente sobre algoritmos, practicar demostraciones, o preparar exámenes escritos.

### Turing — Tutor De Código

**Enfoque:** Conductista con refuerzo progresivo.
**Propósito:** Implementación en Python limpio de algoritmos y estructuras de datos, conectando cada implementación con su análisis formal (invariantes, recurrencias, complejidad).
**Cuándo usarlo:** Cuando necesitas practicar implementaciones, depurar código, o preparar tareas y exámenes de implementación.

### Gauss — Tutor De Apoyo a Asignaciones

**Enfoque:** Aprendizaje Basado en Problemas / Proyectos (ABP/ABPr).
**Propósito:** Guiar al estudiante a comprender, descomponer y resolver tareas, parciales y el Proyecto Final del curso, sin dar la respuesta. Fomenta autonomía y justificación de decisiones.
**Cuándo usarlo:** Cuando tienes un enunciado específico (tarea, taller, parcial, proyecto) y necesitas ayuda para entenderlo, revisar tu avance, o autoevaluar tu entrega antes de enviarla.

**Los 3 tutores mantienen su identidad a lo largo de las 3 temáticas**, permitiendo al estudiante reconocer a Euler, Turing y Gauss como "sus tutores del curso".

---

## Catálogo de Prompts

### Temática 1 — Fundamentos y Grafos Básicos

- `PROMPT-Conceptual-ArbGraf-T1-Fundamentos.md` — Euler (6 niveles: N1-N6)
- `PROMPT-Codigo-ArbGraf-T1-Fundamentos.md` — Turing (7 niveles: N1-N7)
- `PROMPT-Asignacion-ArbGraf-T1-Fundamentos.md` — Gauss (3 modos: A, B, C)

### Temática 2 — Grafos Avanzados

- `PROMPT-Conceptual-ArbGraf-T2-GrafosAvanzados.md` — Euler (7 niveles: N1-N7)
- `PROMPT-Codigo-ArbGraf-T2-GrafosAvanzados.md` — Turing (7 niveles: N1-N7)
- `PROMPT-Asignacion-ArbGraf-T2-GrafosAvanzados.md` — Gauss (3 modos: A, B, C)

### Temática 3 — Árboles, Estructuras Jerárquicas y Cadenas

- `PROMPT-Conceptual-ArbGraf-T3-ArbolesEstructuras.md` — Euler (7 niveles: N1-N7)
- `PROMPT-Codigo-ArbGraf-T3-ArbolesEstructuras.md` — Turing (7 niveles: N1-N7)
- `PROMPT-Asignacion-ArbGraf-T3-ArbolesEstructuras.md` — Gauss (3 modos: A, B, C)

---

## Cómo Usar los Prompts

### Paso 1: Identifica tu necesidad

| Si necesitas... | Usa el tutor... |
|---|---|
| Entender un concepto, razonar formalmente, preparar un examen escrito | **Euler** (Conceptual) |
| Implementar un algoritmo en Python, depurar código, preparar un examen de implementación | **Turing** (De Código) |
| Comprender un enunciado de tarea/parcial/proyecto, revisar tu avance, autoevaluarte antes de entregar | **Gauss** (De Asignaciones) |

### Paso 2: Identifica la temática

| Si el tema es... | Usa la temática... |
|---|---|
| Notación asintótica, invariantes, D&C, búsqueda binaria, grafos básicos, DFS, BFS | **T1** |
| Orden topológico, SCC, puntos de articulación, caminos más cortos (Dijkstra, Bellman-Ford, etc.) | **T2** |
| Árboles, diámetro, Segment Trees, Union-Find, Fenwick, MST, arreglos de sufijos, Proyecto Final | **T3** |

### Paso 3: Copia el prompt y úsalo

1. Abre el archivo `.md` correspondiente.
2. Copia TODO el contenido dentro del bloque ` ``` ` del prompt (desde `1. IDENTIDAD` hasta el final de `10. CIERRE Y REPORTE`).
3. Pégalo como primer mensaje en una conversación con el LLM de tu preferencia.
4. El tutor se presentará y te guiará desde ahí.

### Paso 4: Interactúa con disciplina

- Responde las preguntas del tutor antes de pedir avanzar.
- Si te bloqueas, pide pistas (el tutor tiene un sistema de ayuda escalonada).
- Justifica tus decisiones con argumentos formales, no solo con intuición.
- Al finalizar, pide el **reporte de cierre**: el tutor generará un resumen con tu nivel alcanzado, errores recurrentes y hoja de ruta. Puedes compartirlo con el profesor si lo solicita.

---

## Principios Pedagógicos

Todos los prompts siguen estos principios:

1. **Método Socrático:** Los tutores guían con preguntas, no con respuestas. Nunca entregan soluciones completas.
2. **Ayuda Escalonada:** Tres niveles de pistas — reformulación, pista conceptual, micro-explicación — sin revelar la solución.
3. **Normalización del Error:** Los errores se normalizan antes de señalarse, para evitar bloqueos emocionales ante el rigor matemático.
4. **Práctica de Evocación:** Se pide al estudiante recordar conceptos previos antes de introducir nuevos.
5. **Progresión Estricta:** No se avanza de nivel sin demostrar dominio del actual.
6. **Un Ejercicio a la Vez:** Los tutores nunca dan más de un problema por mensaje.
7. **Rigor Formal:** Se exige notación matemática correcta y demostraciones paso a paso sin saltos lógicos.
8. **Código Limpio:** Todas las implementaciones deben ser en Python 3.7 sin librerías externas, sin `break`, `continue` ni `return` innecesarios, con nombres descriptivos y estructura que refleje el pseudocódigo del CLRS.
9. **Conexión Formal-Implementación:** Después de cada implementación, el estudiante debe poder explicar el invariante, la recurrencia y la complejidad. No basta con que el código funcione.

---

## Requisitos Técnicos

- **Lenguaje:** Python 3.7 exclusivamente.
- **Librerías:** NINGUNA librería externa. Esto incluye `collections`, `heapq`, `deque`, `numpy`, `bisect`, `networkx`, `itertools`, `functools`. Todas las estructuras y algoritmos se implementan desde cero usando solo listas nativas, diccionarios, tuplas y tipos primitivos.
- **Estilo:** Código limpio y legible. Sin `break`, `continue` ni `return` innecesarios. Nombres descriptivos y autoexplicativos.

---

## Reportes de Cierre

Al finalizar una sesión con cualquier tutor, el estudiante puede pedir el **reporte de cierre**. Este reporte incluye:

- **Nivel inicial vs. nivel alcanzado** (para Conceptual y De Código) o **Modo utilizado** (para Asignaciones).
- **Error conceptual o técnico más recurrente.**
- **Calidad del trabajo:** formalismo, código limpio, justificación formal.
- **Uso de explicaciones:** si el estudiante necesitó micro-explicaciones más de 3 veces.
- **Hoja de ruta de aprendizaje:** siguiente paso natural en el curso.

El reporte puede ser compartido con el profesor si lo solicita.

---

## Texto Guía y Referencias

- **Texto principal:** Cormen, T., Leiserson, C., Rivest, R., Stein, C. *Introduction to Algorithms* (Third Edition). MIT Press.
- **Textos adicionales:**
  - Rocha, C. *Diseño y Análisis de Algoritmos* (v0.0).
  - Kleinberg, J., Tardos, É. *Algorithm Design*.
  - Erickson, J. *Algorithms, Etc.* (primera edición, junio 2019).
  - Van Steen, M. *Graph Theory and Complex Networks: An Introduction*.
  - Halim, S., Halim, F., Effendy, S. *Competitive Programming 4*.

---

## Código de Honor

El uso de estos tutores está sujeto al código de honor de la Pontificia Universidad Javeriana Cali. En particular:

- Los tutores NO resuelven las asignaciones. El trabajo entregado debe ser del estudiante.
- Copiar código de otro estudiante, de un tutor virtual, o de cualquier fuente externa y presentarlo como propio constituye plagio.
- El uso del tutor debe documentarse cuando el profesor lo solicite (por ejemplo, incluyendo el reporte de cierre en la entrega).

Para más detalles, consultar el Reglamento de Estudiantes, Sección VI.

---

## Versión

**Versión 1.0** — 2026-1
Generado con el sistema PromptForge (marco de generación de prompts pedagógicos estandarizados para Ingeniería de Sistemas / Ciencias de la Computación de la Pontificia Universidad Javeriana Cali).

# Tutores Virtuales — Infraestructuras Paralelas y Distribuidas

**Universidad del Valle** — Escuela de Ingeniería de Sistemas y Computación
Curso: Infraestructuras Paralelas y Distribuidas (750023C)
Prerrequisito: Fundamentos de Redes (750010C)

---

## Descripción

Este repositorio reúne **7 prompts pedagógicos** que funcionan como tutores virtuales para el curso de Infraestructuras Paralelas y Distribuidas. Cada prompt se copia y se pega en una conversación con un LLM (ChatGPT, Claude, Gemini, etc.), y desde ahí el estudiante recibe acompañamiento socrático.

**Principio fundamental:** los tutores son herramientas de APOYO. El profesor del curso lidera el proceso, acompaña el avance, toma las decisiones académicas y evalúa formalmente. Los tutores NUNCA reemplazan al profesor y NUNCA entregan soluciones completas.

---

## Estructura del Curso

El curso va de paralelizar un programa en una sola máquina a distribuirlo y desplegarlo en varias. Los tutores siguen los dos bloques del campus:

| Bloque | Temas | Resultado de aprendizaje |
|---|---|---|
| **B1 — Programación paralela** | 1. Ley de Amdahl, límites de la paralelización y localidad de caché · 2. Descomposición, granularidad y balanceo (`std::thread`, TBB) · 3. Profiling en Python e instrucciones AVX · 4. Hilos y procesos en Python y el GIL · 5. OpenMP en C++ · 6. Profiling en Linux | R.A.1 — Parcial 1 |
| **B2 — Infraestructuras cloud** | 7. Introducción a los sistemas distribuidos · 8. Docker: imágenes y contenedores · 9. Docker Compose y Swarm · 10. Kubernetes · 11. Pipelines CI/CD con GitHub Actions | R.A.2 y R.A.3 — Parcial 2 |
| **Proyecto final** | Integra paralelización, distribución, despliegue orquestado y CI/CD | R.A.3 |

---

## Los 3 Tutores

### Amdahl — Tutor Conceptual

**Enfoque:** conductista con refuerzo progresivo.
**Propósito:** razonar sobre rendimiento, arquitectura y sistemas distribuidos sin escribir código. Antes de ver un dato, el estudiante predice un número (un *speedup*, una latencia, qué pasa si cae una réplica) y después explica la diferencia con lo que ocurrió.
**Cuándo usarlo:** para entender un concepto, leer una tabla de tiempos o un perfil, o preparar la parte conceptual de un parcial.

### Flynn — Tutor De Código

**Enfoque:** conductista con refuerzo progresivo.
**Propósito:** escribir, paralelizar y medir código en Python y C++ (bloque 1), y escribir `Dockerfile`, `docker-compose.yml`, manifiestos de Kubernetes y *workflows* de GitHub Actions (bloque 2). No sube al mismo tiempo la complejidad de la herramienta y la del problema.
**Cuándo usarlo:** para practicar una herramienta, depurar o preparar los ejercicios de clase.

### Lamport — Tutor De Apoyo a Asignaciones

**Enfoque:** Aprendizaje Basado en Problemas / Proyectos (ABP/ABPr).
**Propósito:** ayudar a entender, avanzar y autoevaluar talleres, opcionales, la preparación de parciales y el proyecto final, sin resolverlos. Trabaja en tres modos: **A** (entender el enunciado), **B** (revisar el avance) y **C** (autoevaluar antes de entregar).
**Cuándo usarlo:** cuando ya hay un enunciado concreto sobre la mesa.

Los tres tutores conservan su identidad en los dos bloques.

---

## Catálogo de Prompts

### Bloque 1 — Programación paralela

- `PROMPT-Conceptual-IPD-B1-ProgramacionParalela.md` — Amdahl (6 niveles: N1-N6)
- `PROMPT-Codigo-IPD-B1-ProgramacionParalela.md` — Flynn (6 niveles: N1-N6)
- `PROMPT-Asignacion-IPD-B1-ProgramacionParalela.md` — Lamport (3 modos: A, B, C)

### Bloque 2 — Infraestructuras cloud

- `PROMPT-Conceptual-IPD-B2-InfraestructurasCloud.md` — Amdahl (6 niveles: N1-N6)
- `PROMPT-Codigo-IPD-B2-InfraestructurasCloud.md` — Flynn (6 niveles: N1-N6)
- `PROMPT-Asignacion-IPD-B2-InfraestructurasCloud.md` — Lamport (3 modos: A, B, C)

### Proyecto final

- `PROMPT-Asignacion-IPD-ProyectoFinal.md` — Lamport (3 modos: A, B, C). Trabaja sobre el enunciado que pegue el grupo.

---

## Cómo Usar los Prompts

### Paso 1: Identifica tu necesidad

| Si necesitas... | Usa el tutor... |
|---|---|
| Entender un concepto, interpretar mediciones, preparar la parte conceptual de un parcial | **Amdahl** (Conceptual) |
| Escribir o depurar código, un `Dockerfile`, un manifiesto o un *workflow* | **Flynn** (De Código) |
| Entender un enunciado, revisar tu avance o autoevaluarte antes de entregar | **Lamport** (De Asignaciones) |

### Paso 2: Identifica el bloque

| Si el tema es... | Usa el bloque... |
|---|---|
| *Speedup*, Amdahl, caché, hilos, procesos, GIL, TBB, OpenMP, AVX, `cProfile`, `perf`, Valgrind | **B1** |
| Sistemas distribuidos, CAP, latencia y *throughput*, Docker, Compose, Kubernetes, GitHub Actions | **B2** |
| El proyecto final del curso | **Proyecto final** |

### Paso 3: Copia el prompt y úsalo

1. Abre el archivo `.md` correspondiente.
2. Copia TODO el contenido del bloque ` ``` ` del prompt (desde `1. IDENTIDAD` hasta el final de `10. CIERRE Y REPORTE`).
3. Pégalo como primer mensaje en una conversación con el LLM que prefieras.
4. El tutor se presenta y te guía desde ahí.

### Paso 4: Interactúa con disciplina

- Responde las preguntas del tutor antes de pedir avanzar.
- Cuando te pida una predicción, escríbela antes de ver el dato.
- Si te bloqueas, pide una pista: el tutor tiene tres niveles de ayuda.
- Justifica con números: un *speedup* sin línea base o una latencia sin percentil no cierran una discusión.
- Al terminar, pide el **reporte de cierre**.

---

## Principios Pedagógicos

1. **Método socrático:** los tutores guían con preguntas y nunca entregan soluciones completas.
2. **Ayuda escalonada:** reformulación, pista conceptual y micro-explicación, sin revelar la solución.
3. **Normalización del error:** el error se nombra como algo frecuente antes de trabajarlo.
4. **Práctica de evocación:** antes de algo nuevo, el tutor pregunta qué recuerdas de lo anterior.
5. **Progresión estricta:** no se sube de nivel sin evidencia de dominio.
6. **Un ejercicio a la vez.**
7. **Medir antes de explicar:** primero la predicción y la medición, después la explicación.
8. **Números coherentes:** las tablas de ejercicio llevan unidades y línea base, y nunca se presentan como mediciones de tu máquina.

---

## Requisitos Técnicos

- **Python 3** con la biblioteca estándar: `threading`, `multiprocessing`, `concurrent.futures`, `cProfile`, `timeit`; además `pyinstrument`.
- **C++17 o superior:** `std::thread`, `std::mutex`, `std::atomic`, Intel TBB, OpenMP. Compilación típica: `g++ -std=c++17 -fopenmp -O2`.
- **Linux:** `top`, `htop`, `ps`, `perf`, Valgrind.
- **Despliegue:** Docker, Docker Compose, minikube o kind, `kubectl`, GitHub Actions.
- En los ejercicios de paralelización manual no se usan NumPy, Numba, Dask ni joblib: esas bibliotecas esconden justo lo que se está practicando.

---

## Reportes de Cierre

Al terminar una sesión con cualquier tutor se puede pedir el **reporte de cierre**, que incluye:

- **Nivel inicial frente a nivel alcanzado** (Conceptual y De Código) o **modo utilizado** (Asignaciones).
- **Error conceptual o técnico más recurrente.**
- **Calidad del trabajo:** manejo de métricas, justificación con números, reproducibilidad.
- **Uso de micro-explicaciones:** si se necesitaron más de 3.
- **Hoja de ruta:** el siguiente paso natural en el curso.

El reporte se comparte con el profesor cuando lo pida.

---

## Referencias

- Tanenbaum, A. S., & van Steen, M. *Distributed Systems*. Van Haren Publishing, 2017.
- McCool, M., Reinders, J., & Robison, A. *Structured Parallel Programming: Patterns for Efficient Computation*. Morgan Kaufmann, 2012.
- Rauber, T., & Rünger, G. *Parallel Programming for Multicore and Cluster Systems* (2.ª ed.). Springer, 2013.
- Documentación oficial de OpenMP, Intel TBB, la biblioteca estándar de Python, Docker, Kubernetes y GitHub Actions.

---

## Uso Honesto

- Los tutores NO resuelven las asignaciones. Lo que se entrega es trabajo del estudiante o del grupo.
- Copiar código, manifiestos o secciones de informe de otro grupo, de un tutor virtual o de cualquier otra fuente y presentarlos como propios es plagio.
- El uso del tutor se documenta cuando el profesor lo pida, por ejemplo, adjuntando el reporte de cierre a la entrega.

Aplica el Reglamento Estudiantil de la Universidad del Valle.

---

## Versión

**Versión 1.0** — 2026-II

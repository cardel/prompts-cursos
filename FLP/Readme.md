# 🤖 Tutores Socráticos - Fundamentos de Interpretación y Compilación de Lenguajes de Programación (FLP)

¡Bienvenido al repositorio de tutores socráticos del curso de FLP! 

Este repositorio contiene una colección de **prompts** (instrucciones preconfiguradas) diseñados para transformar a cualquier modelo de Inteligencia Artificial (como ChatGPT, Claude o Gemini) en un **Tutor Socrático** experto en los temas del curso. 

El objetivo de estos tutores **no es darte la respuesta o hacer el código por ti**, sino guiarte paso a paso, hacerte preguntas clave y ayudarte a razonar sobre la construcción de interpretadores usando Scheme/Racket, basados en el enfoque del libro *Essentials of Programming Languages (EOPL)*.

## 🛠️ ¿Cómo usar estos prompts?

1. Elige el tema que deseas repasar o practicar de la lista de abajo.
2. Abre el archivo `.md` correspondiente en este repositorio.
3. Copia **todo** el contenido del archivo.
4. Pégalo como tu primer mensaje en un chat nuevo de tu IA preferida.
5. ¡Empieza a interactuar! El tutor se presentará y te pedirá que elijas un nivel de dificultad o te propondrá un ejercicio inicial.

> **💡 Tip para estudiantes:** Usa un chat nuevo para cada tutor. Si mezclas a *Lambda* con *Mutare* en la misma conversación, la IA podría confundir las reglas de los entornos.

---

## 📚 Catálogo de Tutores

El curso está dividido en 5 grandes etapas, y cada una cuenta con su propio tutor especializado:

### 1. Lambda 
**Archivo:** `PROMPT-Codigo-FLP-EspecificacionRecursivaDatos-AST.md`
* **Tema:** Especificación recursiva de datos, gramáticas BNF, árboles de sintaxis abstracta (AST), funciones `parse` y `unparse`.
* **Cuándo usarlo:** Cuando estés aprendiendo a definir la sintaxis de tu lenguaje y a transformar código fuente en estructuras de datos manipulables.

### 2. Eval 
**Archivo:** `PROMPT-Codigo-FLP-Interpretador-Clausuras-Recursion.md`
* **Tema:** Construcción del interpretador núcleo, ambientes, condicionales, ligaduras locales (`let`), clausuras, procedimientos y recursión (`letrec`).
* **Cuándo usarlo:** Cuando necesites entender cómo funciona la función `value-of` y cómo se evalúa el código en un ambiente estático.

### 3. Mutare 
**Archivo:** `PROMPT-Codigo-FLP-Estado-Asignacion-PasoParametros.md`
* **Tema:** Estado explícito (Store/Almacén), asignación (`set!`), secuenciación (`begin`) y diferencias entre paso por valor vs. paso por referencia.
* **Cuándo usarlo:** Cuando pases del paradigma funcional puro a introducir efectos colaterales y mutabilidad en tu interpretador.

### 4. Typer 
**Archivo:** `PROMPT-Codigo-FLP-ChequeoInferenciaTipos.md`
* **Tema:** Lenguajes tipados, expresiones de tipo, ambientes de tipos, chequeo estático y algoritmos de inferencia de tipos.
* **Cuándo usarlo:** Cuando estés construyendo la función `type-of` para detectar errores antes de la ejecución del programa.

### 5. Objectum 
**Archivo:** `PROMPT-Codigo-FLP-Objetos-Clases-Herencia.md`
* **Tema:** Objetos simples y planos, clases, campos, métodos, `self`, herencia y *dispatch* de métodos.
* **Cuándo usarlo:** Cuando estés implementando la orientación a objetos dentro de tu interpretador, integrando ambientes, estado y clausuras.

---

## ⚠️ Reglas de Juego (Disclaimer)

* **Mentalidad de crecimiento:** Los tutores te corregirán si tu gramática BNF está mal formada, si confundes el ambiente con el almacén, o si fallas en las reglas de tipado. Aprovecha estos errores para aprender.
* **El profesor tiene la última palabra:** Estos tutores son una herramienta de apoyo al aprendizaje. **NO** reemplazan las directrices de tu profesor. Las evaluaciones formales y decisiones académicas son potestad exclusiva del equipo docente.
* **Codifica, no leas:** La mejor manera de usar estos tutores es tener tu editor de Scheme/Racket abierto a un lado e ir probando el código que construyen juntos.

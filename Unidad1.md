# UNIDAD 1

### [Volver al Portafolio](Portafolio.md)

---


## 1. Resumen teórico

### ¿Qué es la lógica proposicional?
Una **proposición** es un enunciado declarativo (afirmativo o negativo) al que puede asignársele un valor de verdad: **Verdadero (V)** o **Falso (F)**, pero nunca ambos al mismo tiempo. Este principio se denomina **Principio de Bivalencia**.

#### Ejemplos de enunciados:
* $5+3=8$ $\rightarrow$ **SÍ** es proposición (valor de verdad: VERDADERO).
* "La luna es cuadrada" $\rightarrow$ **SÍ** es proposición (valor de verdad: FALSO).
* "¿Qué hora es?" $\rightarrow$ **NO** es proposición (pregunta, no tiene valor V/F).
* "Cierra la puerta" $\rightarrow$ **NO** es proposición (es una orden).
* $x+2=5$ $\rightarrow$ **NO** es proposición (función proposicional: depende de $x$).

---

### Tipos de proposiciones

| Tipo | Descripción | Ejemplo |
| :--- | :--- | :--- |
| **Simple** | Un solo enunciado declarativo sin conectores lógicos. Se simboliza con letras: p, q, r... | $p$: "Hoy es lunes" |
| **Compuesta** | Formada por dos o más proposiciones simples unidas mediante conectores lógicos. | $p \wedge q$: "Hoy es lunes Y no hay clases" |

---

### Conectores Lógicos
Los conectores lógicos (u operadores proposicionales) permiten construir proposiciones compuestas a partir de simples:

| Conector | Símbolo | Se lee como | Ejemplo |
| :--- | :---: | :--- | :--- |
| **Negación** | $\neg p$ | No p | $p$: No llueve |
| **Conjunción** | $p \wedge q$ | p Y q | Llueve $\wedge$ hace frío |
| **Disyunción** | $p \vee q$ | p o q | Llueve $\vee$ hace sol |
| **Condicional** | $p \rightarrow q$ | Si p, entonces q | Estudio $\rightarrow$ apruebo |
| **Bicondicional** | $p \leftrightarrow q$ | p si y solo si q | $p \leftrightarrow q$ ambos iguales |

---

### Tablas de Verdad
Una tabla de verdad muestra sistemáticamente todos los valores de verdad posibles de una proposición compuesta. Con $n$ variables se generan $2^n$ filas de combinaciones.

* **1 variable ($p$):** $2^{1}=2$ filas
* **2 variables ($p, q$):** $2^{2}=4$ filas
* **3 variables ($p, q, r$):** $2^{3}=8$ filas

#### Clasificación según sus resultados:

| Clasificación | Definición | Fórmula clásica |
| :--- | :--- | :--- |
| **Tautología** | Siempre VERDADERA en todos los casos posibles. | $p \vee \neg p \rightarrow \text{siempre V}$ |
| **Contradicción** | Siempre FALSA en todos los casos posibles. | $p \wedge \neg p \rightarrow \text{siempre F}$ |
| **Contingencia** | Puede ser V o F según los valores de sus variables. | $p \rightarrow q \rightarrow \text{depende}$ |

---

### Leyes lógicas
Las leyes proposicionales son equivalencias lógicas ($\equiv$) que permiten transformar y simplificar proposiciones conservando su valor de verdad:

| Ley | Equivalencia |
| :--- | :--- |
| **Doble Negación** | $\neg(\neg p) \equiv p$ |
| **Identidad (A)** | $p \wedge V \equiv p$ |
| **Identidad (V)** | $p \vee F \equiv p$ |
| **Dominación (V)** | $p \vee V \equiv V$ |
| **Dominación (A)** | $p \wedge F \equiv F$ |
| **Idempotencia (V)** | $p \vee p \equiv p$ |
| **Idempotencia (A)** | $p \wedge p \equiv p$ |
| **Conmutativa (V)** | $p \vee q \equiv q \vee p$ |
| **Conmutativa (A)** | $p \wedge q \equiv q \wedge p$ |
| **Asociativa (V)** | $(p \vee q) \vee r \equiv p \vee (q \vee r)$ |
| **Asociativa (A)** | $(p \wedge q) \wedge r \equiv p \wedge (q \wedge r)$ |
| **Distributiva** | $p \vee (q \wedge r) \equiv (p \vee q) \wedge (p \vee r)$ |
| **De Morgan (1)** | $\neg(p \wedge q) \equiv \neg p \vee \neg q$ |
| **De Morgan (2)** | $\neg(p \vee q) \equiv \neg p \wedge \neg q$ |
| **Complemento (V)** | $p \vee \neg p \equiv V$ |
| **Complemento (A)** | $p \wedge \neg p \equiv F$ |
| **Absorción (1)** | $p \vee (p \wedge q) \equiv p$ |
| **Absorción (2)** | $p \wedge (p \vee q) \equiv p$ |

---

### Reglas de Inferencia
Las reglas de inferencia permiten derviar conclusiones válidas a partir de premisas. El símbolo $\therefore$ significa "por lo tanto":

| Regla | Esquema formal | Ejemplo |
| :--- | :--- | :--- |
| **Modus Ponens** | $p \rightarrow q \;/\; p \;/\; \therefore q$ | Si llueve me mojo. Llueve. / Me mojo. |
| **Modus Tollens** | $p \rightarrow q \;/\; \neg q \;/\; \dots \neg p$ | Si llueve me mojo. No me mojo. / No llueve. |
| **Silogismo Hipotético** | $p \rightarrow q \;/\; q \rightarrow r \;/\; \dots p \rightarrow r$ | Estudio apruebo. Apruebo me gradúo. / Estudio me gradúo. |
| **Silogismo Disyuntivo** | $p \vee q \;/\; \neg p \;/\; \dots q$ | Llueve o hace sol. No llueve. / Hace sol. |
| **Simplificación** | $p \wedge q \;/\; \dots p$ | Llueve y hace frío. / Llueve. |
| **Adición** | $p \;/\; \dots p \vee q$ | Llueve. / Llueve o nieva. |

---

## 2. Ejercicios resueltos

### Ejercicio 1
* **Enunciado:** "Si el sensor detecta movimiento y el sistema está activo, entonces suena la alarma".
* **Traducción:**
    * $p$: El sensor detecta movimiento.
    * $q$: El sistema está activo.
    * $r$: Suena la alarma.
    * **Forma simbólica:** $(p \wedge q) \rightarrow r$

#### Tabla de verdad:

| $p$ | $q$ | $r$ | $(p \wedge q)$ | $(p \wedge q) \rightarrow r$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | V | **V** |
| V | V | F | V | **F** |
| V | F | V | F | **V** |
| V | F | F | F | **V** |
| F | V | V | F | **V** |
| F | V | F | F | **V** |
| F | F | V | F | **V** |
| F | F | F | F | **V** |

> **Resultado:** Es una **Contingencia** (hay valores verdaderos y falsos en el resultado final).

---

### Ejercicio 2
* **Traducción:** "O bien el servidor está encendido, o no lo está".
* **Proposición:** $p$: El servidor está encendido.
* **Simbología:** $p \vee \neg p$

#### Tabla de verdad:

| $p$ | $\neg p$ | $p \vee \neg p$ |
| :---: | :---: | :---: |
| V | F | **V** |
| F | V | **V** |

> **Resultado:** Es una **Tautología**. Esta es la *Ley del Tercero Excluido*.

---

### Ejercicio 3
* **Enunciado:** "No es cierto que (llueva o truene), o bien (no llueva y truene)".
* **Proposiciones:** $p$: Llueve, $q$: Truene.
* **Simbología:** $\neg(p \vee q) \vee (\neg p \wedge q)$

#### Aplicación de Leyes (Paso a paso):
1. **De Morgan:** $(\neg p \wedge \neg q) \vee (\neg p \wedge q)$
2. **Distributiva:** $\neg p \wedge (\neg q \vee q)$
3. **Tercero Excluido:** $\neg p \wedge V$
4. **Identidad:** $\neg p$

#### Tabla de verdad simplificada:

| $p$ | $\neg p$ |
| :---: | :---: |
| V | **F** |
| F | **V** |

> **Resultado:** Es una **Contingencia**.

---

### Ejercicio 4
* **Premisa 1 (P1):** Si estudio ($p$), entonces apruebo ($q$).
* **Premisa 2 (P2):** He estudiado ($p$).
* **Conclusión (C):** Por lo tanto, apruebo ($q$).
* **Simbología:** $[(p \rightarrow q) \wedge p] \rightarrow q$

#### Tabla de verdad:

| $p$ | $q$ | $p \rightarrow q$ | $[(p \rightarrow q) \wedge p]$ | $[(p \rightarrow q) \wedge p] \rightarrow q$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | V | **V** |
| V | F | F | F | **V** |
| F | V | V | F | **V** |
| F | F | V | F | **V** |

> **Resultado:** Es una **Tautología**.

---

### Ejemplo 5
* **Traducción:** "El dato es entero y es flotante, y además el dato no es entero".
* **Proposiciones:** $p$: Es entero / $q$: Es flotante.
* **Simbología:** $(p \wedge q) \wedge \neg p$

#### Aplicación de Leyes:
1. **Asociativa y Conmutativa:** $(p \wedge \neg p) \wedge q$
2. **Contradicción:** $F \wedge q$
3. **Dominación:** $F$

#### Tabla de verdad:

| $p$ | $q$ | $(p \wedge q)$ | $\neg p$ | $(p \wedge q) \wedge \neg p$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | F | **F** |
| V | F | F | F | **F** |
| F | V | F | V | **F** |
| F | F | F | V | **F** |

> **Resultado:** Es una **Contradicción**.

---

## 3. Ejercicio aplicado

### Sistema de control de acceso a un laboratorio universitario
**Descripción del problema:** En la universidad, el laboratorio de cómputo aplica las siguientes reglas de acceso:
Un estudiante puede acceder al laboratorio SI cumple alguna de estas condiciones:
1. Tiene carnet universitario vigente Y la puerta está desbloqueada.
2. O si hay un docente presente en el laboratorio.

* **RESTRICCIÓN:** Si el laboratorio está lleno (más de 30 personas), el acceso se niega, aunque se cumplan las condiciones anteriores.

#### Paso 1 - Definir las proposiciones simples:
* $p = $ El estudiante tiene carnet universitario vigente.
* $q = $ La puerta del laboratorio está desbloqueada.
* $r = $ Hay un docente presente en el laboratorio.
* $s = $ El laboratorio tiene más de 30 personas (lleno).
* $A = $ El estudiante puede acceder al laboratorio (conclusión).

#### Paso 2 - Expresar simbólicamente:
* **Regla de acceso base:** $\text{Acceso\_base} = (p \wedge q) \vee r$
* **Regla completa con restricción de capacidad:** $A = [(p \wedge q) \vee r] \wedge \neg s$

> *En lenguaje natural:* "El acceso se permite si (carnet Y puerta abierta) O (docente presente), PERO solo si el laboratorio no está lleno."

#### Paso 3 - Tabla de verdad

| $p$ | $q$ | $r$ | $s$ | $p \wedge q$ | $(p \wedge q) \vee r$ | **Acceso ($A$)** |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| V | V | F | F | V | V | **V** |
| V | F | F | F | F | F | **F** |
| F | F | V | F | F | V | **V** |
| V | V | V | V | V | V | **F** |
| F | F | F | F | F | F | **F** |

#### Paso 4 - Interpretar cada caso:
* **Fila 1** ($p=V, q=V, r=F, s=F$): Carnet + puerta abierta, lab. no lleno $\rightarrow$ **ACCEDE**.
* **Fila 2** ($p=V, q=F, r=F, s=F$): Carnet pero puerta cerrada y sin docente $\rightarrow$ **NO ACCEDE**.
* **Fila 3** ($p=F, q=F, r=V, s=F$): Sin carnet, pero docente presente y espacio $\rightarrow$ **ACCEDE**.
* **Fila 4** ($p=V, q=V, r=V, s=V$): Todo correcto, pero laboratorio LLENO $\rightarrow$ **NO ACCEDE**.
* **Fila 5** (Todo F): No cumple ninguna condición $\rightarrow$ **NO ACCEDE**.

#### Paso 5 - Conclusión:
La lógica proposicional permite modelar formalmente sistemas de control de acceso, políticas institucionales y reglas de negocio. La fórmula $A = [(p \wedge q) \vee r] \wedge \neg s$ expresa con precisión y sin ambigüedad todas las condiciones del sistema. En ingeniería de software, ciberseguridad y sistemas embebidos, este tipo de modelado lógico es fundamental.

---

## 4. Reflexión personal

* **¿Qué fue lo más difícil de entender?**
  Principalmente se me complicó entender y aplicar las leyes lógicas ya que el tema de proposiciones lo había visto por encima en el colegio, pero las leyes han sido algo completamente nuevo en mi conocimiento.

* **¿Qué tema comprendí mejor?**
  No es un tema sino es una parte del tema de la lógica, y son las tablas de verdad, ya que, por curiosidad las vi y estaba algo familiarizado con estas. Otro tema que se me facilitó fueron los conectores lógicos (AND, OR y NOT).

* **¿Cómo puedo aplicar la lógica en mi carrera?**
  Desde un punto de vista aparte la lógica se la aplica siempre ya que es buscar siempre lo más óptimo o saber el valor de algo. Pero viendo a la lógica como el tema que hemos estudiado en la unidad, se la aplica siempre, para ser más exacto a la hora de generar un código: si usamos las leyes lógicas podemos hacer más corto el algoritmo y que funcione igualmente, solo que más rápido, lo que es más óptimo.
## Actividades de la Unidad 1

- [AA - Actividad Autónoma](AAU1.md)
- [ACD - Actividad de Clase/Docente](ACDU1.md)
- [APE - Actividad Práctica de Evaluación](APEU1.md)
- [ES - Evaluación Sumativa](ESU1.md)

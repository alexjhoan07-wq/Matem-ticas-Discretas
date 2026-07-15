# UNIDAD 1

### [Volver al Portafolio](Portafolio.md)

---
# Portafolio de aprendizaje

* [cite_start]**Asignatura:** Matemáticas Discretas [cite: 2]
* [cite_start]**Estudiante:** Jhoan Rojas [cite: 3]
* [cite_start]**Docente:** Mario Cueva Hurtado [cite: 4]
* [cite_start]**Carrera:** Computación [cite: 5]
* [cite_start]**Periodo:** Marzo – Agosto [cite: 6]

---

## [cite_start]1. Resumen teórico [cite: 7]

### [cite_start]¿Qué es la lógica proposicional? [cite: 8]
[cite_start]Una **proposición** es un enunciado declarativo (afirmativo o negativo) al que puede asignársele un valor de verdad: **Verdadero (V)** o **Falso (F)**, pero nunca ambos al mismo tiempo[cite: 9]. [cite_start]Este principio se denomina **Principio de Bivalencia**[cite: 10].

#### [cite_start]Ejemplos de enunciados: [cite: 11]
* [cite_start]$5+3=8$ $\rightarrow$ **SÍ** es proposición (valor de verdad: VERDADERO)[cite: 13].
* [cite_start]"La luna es cuadrada" $\rightarrow$ **SÍ** es proposición (valor de verdad: FALSO)[cite: 13].
* "¿Qué hora es?" [cite_start]$\rightarrow$ **NO** es proposición (pregunta, no tiene valor V/F)[cite: 14].
* [cite_start]"Cierra la puerta" $\rightarrow$ **NO** es proposición (es una orden)[cite: 14].
* [cite_start]$x+2=5$ $\rightarrow$ **NO** es proposición (función proposicional: depende de $x$)[cite: 15].

---

### [cite_start]Tipos de proposiciones [cite: 16]

| Tipo | Descripción | Ejemplo |
| :--- | :--- | :--- |
| **Simple** | Un solo enunciado declarativo sin conectores lógicos. [cite_start]Se simboliza con letras: p, q, r... [cite: 12] | [cite_start]$p$: "Hoy es lunes" [cite: 12] |
| **Compuesta** | [cite_start]Formada por dos o más proposiciones simples unidas mediante conectores lógicos. [cite: 12] | [cite_start]$p \wedge q$: "Hoy es lunes Y no hay clases" [cite: 12] |

---

### [cite_start]Conectores Lógicos [cite: 17]
[cite_start]Los conectores lógicos (u operadores proposicionales) permiten construir proposiciones compuestas a partir de simples[cite: 18, 19]:

| Conector | Símbolo | Se lee como | Ejemplo |
| :--- | :---: | :--- | :--- |
| **Negación** | [cite_start]$\neg p$ [cite: 20] | [cite_start]No p [cite: 20] | [cite_start]$p$: No llueve [cite: 20] |
| **Conjunción** | [cite_start]$p \wedge q$ [cite: 20] [cite_start]| p Y q [cite: 20] | [cite_start]Llueve $\wedge$ hace frío [cite: 20] |
| **Disyunción** | [cite_start]$p \vee q$ [cite: 20] [cite_start]| p o q [cite: 20] | [cite_start]Llueve $\vee$ hace sol [cite: 20] |
| **Condicional** | [cite_start]$p \rightarrow q$ [cite: 20] | [cite_start]Si p, entonces q [cite: 20] | [cite_start]Estudio $\rightarrow$ apruebo [cite: 20] |
| **Bicondicional** | [cite_start]$p \leftrightarrow q$ [cite: 20] [cite_start]| p si y solo si q [cite: 20] | [cite_start]$p \leftrightarrow q$ ambos iguales [cite: 20] |

---

### [cite_start]Tablas de Verdad [cite: 21]
[cite_start]Una tabla de verdad muestra sistemáticamente todos los valores de verdad posibles de una proposición compuesta[cite: 22]. [cite_start]Con $n$ variables se generan $2^n$ filas de combinaciones[cite: 23].

* [cite_start]**1 variable ($p$):** $2^{1}=2$ filas [cite: 25]
* [cite_start]**2 variables ($p, q$):** $2^{2}=4$ filas [cite: 26, 27]
* [cite_start]**3 variables ($p, q, r$):** $2^{3}=8$ filas [cite: 28]

#### [cite_start]Clasificación según sus resultados[cite: 29]:

| Clasificación | Definición | Fórmula clásica |
| :--- | :--- | :--- |
| **Tautología** | [cite_start]Siempre VERDADERA en todos los casos posibles. [cite: 30] | [cite_start]$p \vee \neg p \rightarrow \text{siempre V}$ [cite: 30] |
| **Contradicción** | [cite_start]Siempre FALSA en todos los casos posibles. [cite: 30] | [cite_start]$p \wedge \neg p \rightarrow \text{siempre F}$ [cite: 30] |
| **Contingencia** | [cite_start]Puede ser V o F según los valores de sus variables. [cite: 30] | [cite_start]$p \rightarrow q \rightarrow \text{depende}$ [cite: 30] |

---

### [cite_start]Leyes lógicas [cite: 31]
[cite_start]Las leyes proposicionales son equivalencias lógicas ($\equiv$) que permiten transformar y simplificar proposiciones conservando su valor de verdad[cite: 31]:

| Ley | Equivalencia |
| :--- | :--- |
| **Doble Negación** | [cite_start]$\neg(\neg p) \equiv p$ [cite: 32] |
| **Identidad (A)** | [cite_start]$p \wedge V \equiv p$ [cite: 32] |
| **Identidad (V)** | [cite_start]$p \vee F \equiv p$ [cite: 32] |
| **Dominación (V)** | [cite_start]$p \vee V \equiv V$ [cite: 32] |
| **Dominación (A)** | [cite_start]$p \wedge F \equiv F$ [cite: 32] |
| **Idempotencia (V)** | [cite_start]$p \vee p \equiv p$ [cite: 32] |
| **Idempotencia (A)** | [cite_start]$p \wedge p \equiv p$ [cite: 32] |
| **Conmutativa (V)** | [cite_start]$p \vee q \equiv q \vee p$ [cite: 32] |
| **Conmutativa (A)** | [cite_start]$p \wedge q \equiv q \wedge p$ [cite: 32] |
| **Asociativa (V)** | [cite_start]$(p \vee q) \vee r \equiv p \vee (q \vee r)$ [cite: 32] |
| **Asociativa (A)** | [cite_start]$(p \wedge q) \wedge r \equiv p \wedge (q \wedge r)$ [cite: 32] |
| **Distributiva** | [cite_start]$p \vee (q \wedge r) \equiv (p \vee q) \wedge (p \vee r)$ [cite: 32] |
| **De Morgan (1)** | [cite_start]$\neg(p \wedge q) \equiv \neg p \vee \neg q$ [cite: 32] |
| **De Morgan (2)** | [cite_start]$\neg(p \vee q) \equiv \neg p \wedge \neg q$ [cite: 32] |
| **Complemento (V)** | [cite_start]$p \vee \neg p \equiv V$ [cite: 32] |
| **Complemento (A)** | [cite_start]$p \wedge \neg p \equiv F$ [cite: 32] |
| **Absorción (1)** | [cite_start]$p \vee (p \wedge q) \equiv p$ [cite: 32] |
| **Absorción (2)** | [cite_start]$p \wedge (p \vee q) \equiv p$ [cite: 32] |

---

### [cite_start]Reglas de Inferencia [cite: 33]
[cite_start]Las reglas de inferencia permiten derivar conclusiones válidas a partir de premisas[cite: 34]. [cite_start]El símbolo $\therefore$ significa "por lo tanto"[cite: 35]:

| Regla | Esquema formal | Ejemplo |
| :--- | :--- | :--- |
| **Modus Ponens** | $p \rightarrow q \;/\; p \;/\; [cite_start]\therefore q$ [cite: 36] | Si llueve me mojo. Llueve. [cite_start]/ Me mojo. [cite: 36] |
| **Modus Tollens** | $p \rightarrow q \;/\; \neg q \;/\; [cite_start]\therefore \neg p$ [cite: 36] | Si llueve me mojo. No me mojo. [cite_start]/ No llueve. [cite: 36] |
| **Silogismo Hipotético** | $p \rightarrow q \;/\; q \rightarrow r \;/\; [cite_start]\therefore p \rightarrow r$ [cite: 36] | Estudio apruebo. Apruebo me gradúo. [cite_start]/ Estudio me gradúo. [cite: 36] |
| **Silogismo Disyuntivo** | $p \vee q \;/\; \neg p \;/\; [cite_start]\therefore q$ [cite: 36] | Llueve o hace sol. No llueve. [cite_start]/ Hace sol. [cite: 36] |
| **Simplificación** | $p \wedge q \;/\; [cite_start]\therefore p$ [cite: 36] | Llueve y hace frío. [cite_start]/ Llueve. [cite: 36] |
| **Adición** | $p \;/\; [cite_start]\dots p \vee q$ [cite: 36] | Llueve. [cite_start]/ Llueve o nieva. [cite: 36] |

---

## [cite_start]2. Ejercicios resueltos [cite: 39]

### [cite_start]Ejercicio 1 [cite: 40]
* [cite_start]**Enunciado:** "Si el sensor detecta movimiento y el sistema está activo, entonces suena la alarma"[cite: 41].
* [cite_start]**Traducción:** [cite: 42]
    * [cite_start]$p$: El sensor detecta movimiento[cite: 43].
    * [cite_start]$q$: El sistema está activo[cite: 45].
    * [cite_start]$r$: Suena la alarma[cite: 47].
    * [cite_start]**Forma simbólica:** $(p \wedge q) \rightarrow r$ [cite: 48]

#### [cite_start]Tabla de verdad[cite: 49]:

| $p$ | $q$ | $r$ | $(p \wedge q)$ | $(p \wedge q) \rightarrow r$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | V | [cite_start]**V** [cite: 50] |
| V | V | F | V | [cite_start]**F** [cite: 50] |
| V | F | V | F | [cite_start]**V** [cite: 50] |
| V | F | F | F | [cite_start]**V** [cite: 50] |
| F | V | V | F | [cite_start]**V** [cite: 50] |
| F | V | F | F | [cite_start]**V** [cite: 50] |
| F | F | V | F | [cite_start]**V** [cite: 50] |
| F | F | F | F | [cite_start]**V** [cite: 50] |

> [cite_start]**Resultado:** Es una **Contingencia** (hay valores verdaderos y falsos en el resultado final)[cite: 51].

---

### [cite_start]Ejercicio 2 [cite: 52]
* [cite_start]**Traducción:** "O bien el servidor está encendido, o no lo está"[cite: 54].
* [cite_start]**Proposición:** $p$: El servidor está encendido[cite: 55].
* [cite_start]**Simbología:** $p \vee \neg p$ [cite: 56]

#### [cite_start]Tabla de verdad[cite: 57]:

| $p$ | $\neg p$ | $p \vee \neg p$ |
| :---: | :---: | :---: |
| V | F | [cite_start]**V** [cite: 58] |
| F | V | [cite_start]**V** [cite: 58] |

> [cite_start]**Resultado:** Es una **Tautología**[cite: 59]. [cite_start]Esta es la *Ley del Tercero Excluido*[cite: 60].

---

### [cite_start]Ejercicio 3 [cite: 61]
* [cite_start]**Enunciado:** "No es cierto que (llueva o truene), o bien (no llueva y truene)"[cite: 62].
* [cite_start]**Proposiciones:** $p$: Llueve [cite: 63][cite_start], $q$: Truene[cite: 64].
* [cite_start]**Simbología:** $\neg(p \vee q) \vee (\neg p \wedge q)$ [cite: 65]

#### [cite_start]Aplicación de Leyes (Paso a paso)[cite: 66]:
1. [cite_start]**De Morgan:** $(\neg p \wedge \neg q) \vee (\neg p \wedge q)$ [cite: 67]
2. [cite_start]**Distributiva:** $\neg p \wedge (\neg q \vee q)$ [cite: 68]
3. [cite_start]**Tercero Excluido:** $\neg p \wedge V$ [cite: 69]
4. [cite_start]**Identidad:** $\neg p$ [cite: 70]

#### [cite_start]Tabla de verdad simplificada[cite: 71]:

| $p$ | $\neg p$ |
| :---: | :---: |
| V | [cite_start]**F** [cite: 72] |
| F | [cite_start]**V** [cite: 72] |

> [cite_start]**Resultado:** Es una **Contingencia**[cite: 73].

---

### [cite_start]Ejercicio 4 [cite: 74]
* [cite_start]**Premisa 1 (P1):** Si estudio ($p$), entonces apruebo ($q$)[cite: 76].
* [cite_start]**Premisa 2 (P2):** He estudiado ($p$)[cite: 77].
* [cite_start]**Conclusión (C):** Por lo tanto, apruebo ($q$)[cite: 78].
* [cite_start]**Simbología:** $[(p \rightarrow q) \wedge p] \rightarrow q$ [cite: 79]

#### [cite_start]Tabla de verdad[cite: 80]:

| $p$ | $q$ | $p \rightarrow q$ | $[(p \rightarrow q) \wedge p]$ | $[(p \rightarrow q) \wedge p] \rightarrow q$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | V | [cite_start]**V** [cite: 81] |
| V | F | F | F | [cite_start]**V** [cite: 81] |
| F | V | V | F | [cite_start]**V** [cite: 81] |
| F | F | V | F | [cite_start]**V** [cite: 81] |

> [cite_start]**Resultado:** Es una **Tautología**[cite: 82].

---

### [cite_start]Ejemplo 5 [cite: 83]
* [cite_start]**Traducción:** "El dato es entero y es flotante, y además el dato no es entero"[cite: 84].
* [cite_start]**Proposiciones:** $p$: Es entero / $q$: Es flotante[cite: 86].
* [cite_start]**Simbología:** $(p \wedge q) \wedge \neg p$ [cite: 87]

#### [cite_start]Aplicación de Leyes[cite: 88]:
1. [cite_start]**Asociativa y Conmutativa:** $(p \wedge \neg p) \wedge q$ [cite: 89]
2. [cite_start]**Contradicción:** $F \wedge q$ [cite: 90]
3. [cite_start]**Dominación:** $F$ [cite: 91]

#### [cite_start]Tabla de verdad[cite: 92]:

| $p$ | $q$ | $(p \wedge q)$ | $\neg p$ | $(p \wedge q) \wedge \neg p$ |
| :---: | :---: | :---: | :---: | :---: |
| V | V | V | F | [cite_start]**F** [cite: 93] |
| V | F | F | F | [cite_start]**F** [cite: 93] |
| F | V | F | V | [cite_start]**F** [cite: 93] |
| F | F | F | V | [cite_start]**F** [cite: 93] |

> [cite_start]**Resultado:** Es una **Contradicción**[cite: 94].

---

## [cite_start]3. Ejercicio aplicado [cite: 95]

### [cite_start]Sistema de control de acceso a un laboratorio universitario [cite: 96]
[cite_start]**Descripción del problema:** En la universidad, el laboratorio de cómputo aplica las siguientes reglas de acceso[cite: 97]:
[cite_start]Un estudiante puede acceder al laboratorio SI cumple alguna de estas condiciones[cite: 98]:
1. [cite_start]Tiene carnet universitario vigente Y la puerta está desbloqueada[cite: 99].
2. [cite_start]O si hay un docente presente en el laboratorio[cite: 100].

* [cite_start]**RESTRICCIÓN:** Si el laboratorio está lleno (más de 30 personas), el acceso se niega, aunque se cumplan las condiciones anteriores[cite: 101, 102].

#### [cite_start]Paso 1 - Definir las proposiciones simples: [cite: 103]
* [cite_start]$p = $ El estudiante tiene carnet universitario vigente[cite: 105].
* [cite_start]$q = $ La puerta del laboratorio está desbloqueada[cite: 105].
* [cite_start]$r = $ Hay un docente presente en el laboratorio[cite: 106].
* [cite_start]$s = $ El laboratorio tiene más de 30 personas (lleno)[cite: 107].
* [cite_start]$A = $ El estudiante puede acceder al laboratorio (conclusión)[cite: 108].

#### [cite_start]Paso 2 - Expresar simbólicamente: [cite: 109]
* [cite_start]**Regla de acceso base:** $\text{Acceso\_base} = (p \wedge q) \vee r$ [cite: 111]
* [cite_start]**Regla completa con restricción de capacidad:** $A = [(p \wedge q) \vee r] \wedge \neg s$ [cite: 113]

> [cite_start]*En lenguaje natural:* "El acceso se permite si (carnet Y puerta abierta) O (docente presente), PERO solo si el laboratorio no está lleno." [cite: 114]

#### [cite_start]Paso 3 - Tabla de verdad [cite: 115]

| $p$ | $q$ | $r$ | $s$ | $p \wedge q$ | $(p \wedge q) \vee r$ | **Acceso ($A$)** |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| V | V | F | F | V | V | [cite_start]**V** [cite: 116] |
| V | F | F | F | F | F | [cite_start]**F** [cite: 116] |
| F | F | V | F | F | V | [cite_start]**V** [cite: 116] |
| V | V | V | V | V | V | [cite_start]**F** [cite: 116] |
| F | F | F | F | F | F | [cite_start]**F** [cite: 116] |

#### [cite_start]Paso 4 - Interpretar cada caso: [cite: 117]
* [cite_start]**Fila 1** ($p=V, q=V, r=F, s=F$): Carnet + puerta abierta, lab. no lleno $\rightarrow$ **ACCEDE**[cite: 118].
* [cite_start]**Fila 2** ($p=V, q=F, r=F, s=F$): Carnet pero puerta cerrada y sin docente $\rightarrow$ **NO ACCEDE**[cite: 120].
* [cite_start]**Fila 3** ($p=F, q=F, r=V, s=F$): Sin carnet, pero docente presente y espacio $\rightarrow$ **ACCEDE**[cite: 121].
* [cite_start]**Fila 4** ($p=V, q=V, r=V, s=V$): Todo correcto, pero laboratorio LLENO $\rightarrow$ **NO ACCEDE**[cite: 122].
* [cite_start]**Fila 5** (Todo F): No cumple ninguna condición $\rightarrow$ **NO ACCEDE**[cite: 123].

#### [cite_start]Paso 5 - Conclusión: [cite: 124]
[cite_start]La lógica proposicional permite modelar formalmente sistemas de control de acceso, políticas institucionales y reglas de negocio[cite: 125]. [cite_start]La fórmula $A = [(p \wedge q) \vee r] \wedge \neg s$ expresa con precisión y sin ambigüedad todas las condiciones del sistema[cite: 126]. [cite_start]En ingeniería de software, ciberseguridad y sistemas embebidos, este tipo de modelado lógico es fundamental[cite: 127].

---

## [cite_start]4. Reflexión personal [cite: 128]

* [cite_start]**¿Qué fue lo más difícil de entender?** [cite: 129]
  [cite_start]Principalmente se me complicó entender y aplicar las leyes lógicas ya que el tema de proposiciones lo había visto por encima en el colegio, pero las leyes han sido algo completamente nuevo en mi conocimiento[cite: 130].

* [cite_start]**¿Qué tema comprendí mejor?** [cite: 131]
  [cite_start]No es un tema sino es una parte del tema de la lógica, y son las tablas de verdad, ya que, por curiosidad las vi y estaba algo familiarizado con estas[cite: 132]. [cite_start]Otro tema que se me facilitó fueron los conectores lógicos (AND, OR y NOT)[cite: 133].

* [cite_start]**¿Cómo puedo aplicar la lógica en mi carrera?** [cite: 134]
  [cite_start]Desde un punto de vista aparte la lógica se la aplica siempre ya que es buscar siempre lo más óptimo o saber el valor de algo[cite: 135]. [cite_start]Pero viendo a la lógica como el tema que hemos estudiado en la unidad, se la aplica siempre, para ser más exacto a la hora de generar un código: si usamos las leyes lógicas podemos hacer más corto el algoritmo y que funcione igualmente, solo que más rápido, lo que es más óptimo[cite: 136].

## Actividades de la Unidad 1

- [AA - Actividad Autónoma](AAU1.md)
- [ACD - Actividad de Clase/Docente](ACDU1.md)
- [APE - Actividad Práctica de Evaluación](APEU1.md)
- [ES - Evaluación Sumativa](ESU1.md)

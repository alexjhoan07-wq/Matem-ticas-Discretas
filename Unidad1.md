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
| **Dominación (V)**

## Actividades de la Unidad 1

- [AA - Actividad Autónoma](AAU1.md)
- [ACD - Actividad de Clase/Docente](ACDU1.md)
- [APE - Actividad Práctica de Evaluación](APEU1.md)
- [ES - Evaluación Sumativa](ESU1.md)

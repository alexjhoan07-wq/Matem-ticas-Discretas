# UNIDAD 3

### [Volver al Portafolio](Portafolio.md)

---

# Unidad 3: Teoría de Grafos y Árboles


---

## Resumen teórico

### Concepto de Grafo
Un grafo se formaliza matemáticamente como una terna $G = (V, E, \varphi)$. En esta estructura, $V$ representa un conjunto finito de elementos llamados vértices o nodos, $E$ es el conjunto de conexiones denominadas aristas, y $\varphi$ es la función de incidencia que vincula de manera única cada arista con un par de vértices.

### Vocabulario Esencial
- **Orden del Grafo:** Se refiere a la cantidad de vértices que contiene el grafo ($|V|$).
- **Tamaño del Grafo:** Es el número total de aristas o enlaces existentes ($|E|$).
- **Grado o Valencia:** Indica cuántas aristas se conectan directamente a un nodo específico.

### Clasificación de Recorridos
- **Recorrido Euleriano:** Consiste en transitar por cada una de las aristas del grafo exactamente una vez. Para que un grafo conexo contenga un ciclo euleriano, es requisito indispensable que todos sus nodos posean un grado par.
- **Recorrido Hamiltoniano:** Se basa en visitar cada uno de los vértices del grafo una única vez. Determinar la existencia de este camino constituye un desafío algorítmico catalogado como problema NP-completo.

### Algoritmos para la Toma de Decisiones y Optimización
- **Algoritmo de Fleury:** Una estrategia paso a paso diseñada para identificar trayectos eulerianos, asegurando que solo se crucen "puentes" (aristas críticas de desconexión) cuando no queden otras alternativas de paso.
- **Algoritmo de Dijkstra:** Método de exploración que calcula la ruta de menor costo entre un nodo de origen y los demás nodos, aplicable en sistemas con aristas de peso no negativo mediante el uso de etiquetas de control temporales y definitivas.

### Modelado Numérico de Grafos
Los entornos informáticos se apoyan en matrices para procesar estas estructuras:
- **Matriz de Adyacencia:** Representación cuadrada de dimensiones $V \times V$. Es la herramienta estándar para descifrar el número de rutas posibles de longitud $k$ a través del cálculo de potencias matriciales.
- **Matriz de Incidencia:** Tabla rectangular de dimensiones $V \times E$ que mapea vértices contra aristas, resultando de gran utilidad en la representación de multigrafos.

### Teoría de Árboles
Un árbol se define como un grafo que cumple las propiedades de ser conexo y no contener ciclos (acíclico). Dentro del área de la computación, destacan los árboles binarios de búsqueda (BST) y sus métodos de recorrido:
* **Preorden:** Visita la raíz, luego el subárbol izquierdo y finalmente el derecho.
* **Inorden:** Explora el subárbol izquierdo, evalúa la raíz y luego el subárbol derecho.
* **Posorden:** Recorre el subárbol izquierdo, el derecho y por último procesa la raíz.

---

## Ejercicios resueltos (Adaptados del Trabajo Autónomo)

### Ejercicio 1: Límites Estructurales de Aristas

**Planteamiento:** Determinar el número máximo de aristas posibles para tres escenarios estructurales distintos con un total de **12 vértices ($n = 12$)**:
1. Un grafo simple cualquiera.
2. Un grafo bipartito completo.
3. Un árbol.

**Desarrollo:**
* **Caso 1 (Grafo Completo $K_{12}$):** La cota máxima de conexiones se produce cuando todos los nodos se enlazan mutuamente. Aplicando la fórmula:
  $$\text{Aristas Máximas} = \frac{n(n - 1)}{2} = \frac{12 \times 11}{2} = 66 \text{ aristas}$$
* **Caso 2 (Grafo Bipartito Completo $K_{6,6}$):** El límite de aristas se maximiza distribuyendo los 12 vértices de forma perfectamente equitativa en dos subconjuntos independientes de 6 elementos cada uno ($V_1 = 6, V_2 = 6$).
  $$\text{Aristas Máximas} = |V_1| \times |V_2| = 6 \times 6 = 36 \text{ aristas}$$
* **Caso 3 (Árbol de 12 nodos):** Por definición, un árbol conexo y acíclico de orden $n$ cuenta estrictamente con una arista menos que su cantidad de nodos para evitar la formación de ciclos.
  $$\text{Aristas Máximas} = n - 1 = 12 - 1 = 11 \text{ aristas}$$

**Conclusión:** Un sistema de 12 nodos soportará como máximo 66 aristas si es totalmente libre, 36 si está restringido por bipartición, y exactamente 11 si adopta una estructura de árbol.

---

### Ejercicio 2: Caracterización de Poliedros y Grafos Planos

**Planteamiento:** Un poliedro convexo posee **14 caras en total ($f = 14$)**. Sabemos que 8 de estas caras son de forma triangular (3 lados) y 5 de ellas son cuadriláteros (4 lados). Si el cuerpo geométrico cuenta con **13 vértices ($v = 13$)**:
1. ¿Cuál es el número total de aristas ($e$) del poliedro?
2. ¿Cuántos lados posee la última cara restante (la cara misteriosa)?

**Desarrollo:**
1. **Cálculo de Aristas:** Empleamos la fórmula de Euler para redes planas y poliedros convexos ($v - e + f = 2$):
   $$13 - e + 14 = 2 \implies e = 13 + 14 - 2 = 25 \text{ aristas}$$
2. **Determinación de los Lados de la Cara Misteriosa:** Como cada arista sirve de frontera común a exactamente dos caras, la suma total de los lados de todas las caras individuales del poliedro es igual a $2 \times e$:
   $$\text{Suma total de lados} = 2 \times 25 = 50 \text{ lados}$$
   - Las 8 caras triangulares aportan: $8 \times 3 = 24$ lados.
   - Las 5 caras cuadrangulares aportan: $5 \times 4 = 20$ lados.
   - Subtotal de lados conocidos: $24 + 20 = 44$ lados.
   - Lados de la cara misteriosa: $50 - 44 = 6$ lados.

**Conclusión:** La cara restante del poliedro posee **6 lados**, lo que significa que es un **hexágono**.

---

### Ejercicio 3: Demostración del Número Cromático en Árboles

**Planteamiento:** Demostrar analítica e inductivamente que el número cromático de cualquier árbol que contenga al menos un canal de comunicación (una arista) es exactamente igual a **2** ($\chi(T) = 2$).

**Desarrollo:**
1. **Algoritmo de Coloreado Dinámico:** Seleccionamos un nodo cualquiera como la raíz y le asignamos el color *A*. Sus nodos descendientes directos (nivel 1) reciben el color *B*. Los descendientes de estos (nivel 2) regresan al color *A*, alternando progresivamente según la paridad de la distancia a la raíz. Dado que un árbol carece de bucles o ciclos, los únicos nodos que comparten una arista obligatoriamente se encuentran en niveles consecutivos, garantizando que nunca tengan el mismo color.
2. **Prueba Inductiva:**
   - **Caso Base ($n = 2$):** Un árbol elemental con dos vértices conectados por una sola arista se puede colorear perfectamente usando dos colores diferentes, lo cual cumple la propiedad $\chi(T) \le 2$.
   - **Hipótesis de Inducción:** Suponemos que cualquier árbol con $k$ nodos puede ser coloreado sin conflictos utilizando a lo sumo 2 colores.
   - **Paso Inductivo ($k + 1$ nodos):** Sea $T$ un árbol con $k + 1$ vértices. Al ser un árbol, existe por lo menos un vértice de grado 1 (un nodo terminal u "hoja"). Al remover temporalmente esta hoja $v$, el grafo resultante $T'$ tiene $k$ vértices, por lo que hereda una coloración válida con 2 colores debido a nuestra hipótesis de inducción. Al reincorporar a $v$, como este solo se conecta con un único nodo padre en el árbol original, basta con asignarle el color opuesto al de su padre para completar el coloreado sin conflictos.

**Conclusión:** Se comprueba inductivamente que todo árbol tiene un número cromático idéntico a 2.

---

### Ejercicio 4: Existencia de Recorridos Hamiltonianos en Grafos Completos

**Planteamiento:** Determinar para qué valores del orden $n$ el grafo completo $K_n$ garantiza la existencia de:
1. Un camino de Hamilton.
2. Un ciclo de Hamilton.

**Desarrollo:**
1. **Camino de Hamilton:** En un grafo completo de orden $n$, cada nodo se encuentra enlazado directamente con todos los demás de la estructura. Debido a esto, cualquier permutación o secuencia aleatoria de sus $n$ vértices constituye una ruta transitable. Por consiguiente, $K_n$ alberga un camino de Hamilton para cualquier valor de **$n \ge 1$**.
2. **Ciclo de Hamilton:** Para configurar un ciclo, el recorrido exige poder regresar al nodo inicial cerrando una trayectoria poligonal simple, lo cual matemáticamente requiere de al menos 3 vértices distintos. Al ser un grafo completo con adyacencia total, cualquier ordenamiento cerrado es factible siempre y cuando se cumpla que **$n \ge 3$**.

| Orden ($n$) | ¿Camino de Hamilton? | ¿Ciclo de Hamilton? | Secuencia ejemplo |
|:---:|:---:|:---:|:---:|
| $n = 1$ | Sí (trivial) | No | $1$ |
| $n = 2$ | Sí | No | $1 \rightarrow 2$ |
| $n = 3$ | Sí | Sí | $1 \rightarrow 2 \rightarrow 3 \rightarrow 1$ |
| $n = 4$ | Sí | Sí | $1 \rightarrow 2 \rightarrow 3 \rightarrow 4 \rightarrow 1$ |

**Conclusión:** Un grafo completo $K_n$ contiene caminos hamiltonianos para todo $n \ge 1$, y ciclos hamiltonianos para todo $n \ge 3$.

---

### Ejercicio 5: Modelado de Distribución Física (Mesa Redonda)

**Planteamiento:** Un grupo de 6 desarrolladores de software necesita sentarse alrededor de una mesa de reuniones circular. Se requiere que cada desarrollador quede flanqueado directamente por dos colegas con quienes tenga compatibilidad técnica de trabajo (representada como una arista en un grafo de compatibilidad). Explica la relación de esta distribución con la teoría de recorridos en grafos.

**Desarrollo:**
1. **Modelado Teórico:** Situar a cada persona entre dos contactos compatibles en una mesa cerrada exige recorrer cada uno de los nodos (desarrolladores) de la red de compatibilidad una sola vez, para retornar finalmente al primero.
2. **Identificación del Recorrido:**
   - Este problema se asocia de forma directa con la búsqueda de un **ciclo de Hamilton** en el grafo de relaciones, ya que la prioridad absoluta recae sobre la visita única a los vértices (las personas).
   - **Diferencia Clave:** No se debe confundir con un circuito de Euler. El circuito de Euler obligaría a emplear cada conexión o arista del sistema exactamente una vez, lo cual es innecesario aquí, ya que varias relaciones de compatibilidad quedarán sin usarse al sentar a los desarrolladores en la mesa.

**Conclusión:** La distribución física planteada es realizable si y solo si el grafo de compatibilidades posee un ciclo de Hamilton.

---

### Ejercicio 6: Emparejamientos Perfectos y Teoría de Grafos

**Planteamiento:** 1. ¿Bajo qué condiciones un grafo completo $K_n$ dispone de un emparejamiento perfecto (*matching perfecto*)?
2. Demostrar que para que un grafo cualquiera posea un matching perfecto, su número de vértices $|V|$ tiene que ser obligatoriamente un número par.
3. Analizar si la condición de que $|V|$ sea par resulta suficiente para asegurar que un grafo cuente con un matching perfecto.

**Desarrollo:**
1. **Condición en $K_n$:** En un grafo completo de orden $n$, cada nodo tiene una arista con todos los demás, de manera que es factible emparejar los elementos de cualquier forma. No obstante, al agrupar los elementos de dos en dos, se requiere estrictamente que **$n$ sea una cifra par**.
2. **Demostración Analítica:** Si un grafo $G$ admite un matching perfecto $M$, esto significa por definición que existe un conjunto de aristas donde cada nodo de $V$ pertenece a una única arista de $M$, sin solapamiento alguno. Al estar conformado cada enlace por exactamente dos extremos, se cumple que:
   $$|V| = 2 \times |M|$$
   Al ser $|M|$ un número entero, la multiplicación asegura que el tamaño del conjunto $|V|$ es un múltiplo de dos y, por ende, par.
3. **Análisis de Suficiencia (El Recíproco):** Que $|V|$ sea par **no es una condición suficiente** para garantizar el matching. Como contraejemplo, consideremos un grafo con 6 vértices ($|V| = 6$ es par) donde un nodo se encuentra totalmente aislado (grado 0) y los otros 5 forman un pentágono conexo. Dado que el vértice aislado carece de canales de conexión con el resto de la estructura, es físicamente imposible incluirlo en algún emparejamiento, imposibilitando un matching perfecto para el grafo global.

**Conclusión:** Un orden de vértices par es un requisito obligatorio (necesario) pero no basta por sí solo (no es suficiente) para garantizar que un grafo admita un emparejamiento perfecto.

---

## Ejercicio aplicado en un caso real

### Planteamiento del problema
Se modeló una red de distribución de datos de una pequeña oficina compuesta por 8 terminales de red (nodos), donde las conexiones físicas (aristas) representan la velocidad de transmisión de datos medida en milisegundos de latencia (peso).

### Análisis con lógica y grafos
- **Vértices:** Servidor, Terminal_A, Terminal_B, Switch_1, Router_Core, Terminal_C, Switch_2, Firewall.
- **Grado de Conexión:** El grafo que modela la oficina es conexo, lo que asegura que todas las terminales disponen de un canal de comunicación activo con la red.
- **Nodos Críticos:** Tras realizar pruebas de conectividad, se determinó que los nodos "Switch_1", "Router_Core" y "Switch_2" son esenciales. Una falla en cualquiera de estos puntos provocaría la desconexión total de amplios sectores de la oficina.

### Resultado del análisis
Aplicando el algoritmo de Dijkstra, se calculó la ruta más eficiente y con menor pérdida de tiempo (menor latencia acumulada) para transmitir un paquete desde el "Servidor" hasta el nodo "Firewall". La secuencia óptima identificada fue:
$$\text{Servidor} \rightarrow \text{Switch\_1} \rightarrow \text{Router\_Core} \rightarrow \text{Switch\_2} \rightarrow \text{Firewall}$$
Garantizando un tiempo mínimo de respuesta de **15 ms**.

---

## Reflexión personal

### ¿Qué fue lo más difícil de entender?
El mayor obstáculo de aprendizaje radicó en asimilar las diferencias de fondo entre los recorridos eulerianos (enfocados en el paso por aristas sin repetición) y los recorridos hamiltonianos (enfocados en la visita a vértices). De igual manera, asimilar la teoría detrás de la clasificación NP-completa de los ciclos hamiltonianos supuso un esfuerzo conceptual demandante.

### ¿Qué temas comprendí mejor?
Considero que asimilé con gran facilidad la representación matricial de estructuras de red (específicamente la matriz de adyacencia), descubriendo cómo la aplicación de conceptos algebraicos como las potencias de matrices simplifica en gran medida el cálculo exacto del número de conexiones posibles de longitud $k$.

### ¿Cómo puedo aplicar la teoría de grafos en mi carrera?
En el ámbito de la computación, la teoría de grafos se perfila como una herramienta indispensable para estructurar bases de datos optimizadas (como las bases de datos orientadas a grafos), optimizar topologías y cableados lógicos en redes de comunicación, y diseñar motores de búsqueda de rutas eficaces para sistemas de posicionamiento global (GPS).

---



## Actividades de la Unidad 3

- [AA - Actividad Autónoma](AAU3.md)
- [ACD - Actividad de Clase/Docente](ACDU3.md)
- [APE - Actividad Práctica de Evaluación](APEU3.md)
- [ES - Evaluación Sumativa](ESU3.md)

- [Regresar a la Portada](Portafolio.md)

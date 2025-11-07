# Nombre: Carlos Alfonso Llanes
# Materia: Fundamentos de Álgebra
# Mtro: Jorge Javier Pedrozo
# Fecha: 7/11/2025
# Grupo: 1C


# Álgebra Lineal — Ejercicios de Matrices (07/11/2025)

---

## Objetivo de la documentación


## Ejercicios realizados

### Ejercicio 1 — Clasificar matrices

## Identificar Matriz
#### Matriz 1
- **Tipo:** Matriz identidad.  
- **Justificación:** *Es matriz identidad porque los elementos de la diagonal son 1 y los demás elementos son 0.*  

Matriz: 
$`\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}`$


---

#### Matriz 2
- **Tipo:** Matriz diagonal.  
- **Justificación:** *Es matriz diagonal porque los elementos de la diagonal son diferentes y los valores afuera de la diagonal son 0.*  

Matriz:  
$`\begin{bmatrix} 3 & 0 & 0 \\ 0 & -2 & 0 \\ 0 & 0 & 5 \end{bmatrix}`$

---

#### Matriz 3
- **Tipo:** Matriz simétrica.  
- **Justificación:** *Es matriz simétrica porque es igual a su transpuesta.*  

Matriz:  
$`\begin{bmatrix} 2 & 1 & 4 \\ 1 & 3 & 5 \\ 4 & 5 & 6 \end{bmatrix}`$

---

#### Matriz 4
- **Tipo:** Matriz triangular superior.  
- **Justificación:** *Es matriz triangular superior porque todos los elementos debajo de la diagonal son 0.*  

Matriz:  
$`\begin{bmatrix} 1 & 2 & 3 \\ 0 & 4 & 5 \\ 0 & 0 & 6 \end{bmatrix}`$

---

### Ejercicio 2 — Operaciones básicas

**Enunciado (Resumen):** Dados \(A\) y \(B\), calcular la suma, la combinación lineal \(2A-B\), los productos \(AB\) y \(BA\), y la traspuesta \(A^T\).  
Mostrar procedimiento elemento a elemento para cada operación.

**Matrices:**

$`\qquad A = \begin{bmatrix} 2 & -1 \\ 3 & 4 \end{bmatrix}`$
$`\qquad B = \begin{bmatrix} 5 & 2 \\ -1 & 3 \end{bmatrix} `$

---

#### a) \(A + B\)

$` \qquad (A+B) = \begin{bmatrix} 2+5 & -1+2 \\ 3+(-1) & 4+3 \end{bmatrix} `$ $` = \begin{bmatrix} 7 & 1 \\ 2 & 7 \end{bmatrix} `$

---

#### b) \(2A - B\)

$` \qquad 2A = \begin{bmatrix} 4 & -2 \\ 6 & 8 \end{bmatrix} `$ $` \quad 2A - B = \begin{bmatrix} 4-5 & -2-2 \\ 6-(-1) & 8-3 \end{bmatrix} `$ $` = \begin{bmatrix} -1 & -4 \\ 7 & 5 \end{bmatrix} `$

---

#### c) \(AB\)

$` AB = \begin{bmatrix} 2\cdot5 + (-1)\cdot(-1) & 2\cdot2 + (-1)\cdot3 \\ 3\cdot5 + 4\cdot(-1) & 3\cdot2 + 4\cdot3 \end{bmatrix} `$ $` = \begin{bmatrix} 11 & 1 \\ 11 & 18 \end{bmatrix} `$

---

#### d) \(BA\)

$` BA = \begin{bmatrix} 5\cdot2 + 2\cdot3 & 5\cdot(-1) + 2\cdot4 \\ (-1)\cdot2 + 3\cdot3 & (-1)\cdot(-1) + 3\cdot4 \end{bmatrix} = \begin{bmatrix} 16 & 3 \\ 7 & 13 \end{bmatrix} `$

> **Observación:** \(AB \neq BA\) → la multiplicación de matrices **no es conmutativa**.

---

#### e) \(A^T\)

$` A^T = \begin{bmatrix} 2 & 3 \\ -1 & 4 \end{bmatrix} `$

---

### Ejercicio 3 — Multiplicación en cadena (asociatividad)

**Enunciado (Resumen):** Comprobar que \((AB)C = A(BC)\) y mostrar procedimiento completo.

**Matrices:**

$$` A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad B = \begin{bmatrix} 2 & 0 \\ 1 & 3 \end{bmatrix}, \quad C = \begin{bmatrix} 1 & 1 \\ 0 & 2 \end{bmatrix} `$$

---

#### Paso 1: Calcular \(AB\)

$` AB = \begin{bmatrix} 1\cdot2 + 2\cdot1 & 1\cdot0 + 2\cdot3 \\ 3\cdot2 + 4\cdot1 & 3\cdot0 + 4\cdot3 \end{bmatrix} = \begin{bmatrix} 4 & 6 \\ 10 & 12 \end{bmatrix} `$

---

#### Paso 2: Calcular \((AB)C\)

$` (AB)C = \begin{bmatrix} 4\cdot1 + 6\cdot0 & 4\cdot1 + 6\cdot2 \\ 10\cdot1 + 12\cdot0 & 10\cdot1 + 12\cdot2 \end{bmatrix} = \begin{bmatrix} 4 & 16 \\ 10 & 34 \end{bmatrix} `$

---

#### Paso 3: Calcular \(BC\)

$` BC = \begin{bmatrix} 2\cdot1 + 0\cdot0 & 2\cdot1 + 0\cdot2 \\ 1\cdot1 + 3\cdot0 & 1\cdot1 + 3\cdot2 \end{bmatrix} = \begin{bmatrix} 2 & 2 \\ 1 & 7 \end{bmatrix} `$

---

#### Paso 4: Calcular \(A(BC)\)

$` A(BC) = \begin{bmatrix} 1\cdot2 + 2\cdot1 & 1\cdot2 + 2\cdot7 \\ 3\cdot2 + 4\cdot1 & 3\cdot2 + 4\cdot7 \end{bmatrix} = \begin{bmatrix} 4 & 16 \\ 10 & 34 \end{bmatrix} `$

---

#### Resultado y conclusión

$` (AB)C = A(BC) = \begin{bmatrix} 4 & 16 \\ 10 & 34 \end{bmatrix} `$

Por lo tanto, se cumple la **propiedad asociativa** en la multiplicación de matrices.

---




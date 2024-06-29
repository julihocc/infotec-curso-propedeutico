---
marp: true
theme: uncover
author: Prof. Juliho Castillo Colmenares Ph.D.
title: Álgebra Lineal
description: Curso propedéutico de Computación
---

### Tutorial: Operaciones Básicas con Matrices en Numpy

---

#### 1. **Creación de Matrices**
- **`np.array()`**: Para crear una matriz, simplemente pasa una lista o tupla como argumento.
  ```python
  matriz = np.array([[1, 2], [3, 4]])
  ```

- **`np.matrix()`**: Otra forma de crear matrices, aunque `np.array()` es más recomendado.
  ```python
  matriz = np.matrix([[1, 2], [3, 4]])
  ```

----

#### 2. **Multiplicación Matricial**
- **`A @ B` o `np.dot(A, B)`**: Para multiplicar matrices A y B matricialmente.
  
  ```python
  resultado = A @ B
  ```
  
- **`A * B` o `np.multiply(A, B)`**: Para multiplicar matrices elemento a elemento.

---

#### 3. **Determinante de una Matriz**
- **`np.det()`**: Calcula el determinante de una matriz.
  ```python
  det = np.linalg.det(matriz)
  ```

---

#### 4. **Acceder a Elementos de una Matriz**
- Las matrices en Numpy usan indexación basada en 0. Para acceder al elemento en la segunda fila y tercera columna:
  ```python
  elemento = matriz[1, 2]
  ```

---

#### 5. **Matrices Identidad**
- **`np.eye()` o `np.identity()`**: Crea una matriz identidad del tamaño especificado.
  ```python
  identidad = np.eye(4)
  ```

---

#### 6. **Transpuesta de una Matriz**
- **`.T` o `np.transpose()`**: Obtiene la transpuesta de una matriz.
  ```python
  transpuesta = matriz.T
  ```

---

#### 7. **Inversa de una Matriz**
- **`np.inv()`**: Calcula la inversa de una matriz.
  ```python
  inversa = np.linalg.inv(matriz)
  ```

---

#### 8. **Eigenvalores y eigenvectores**

- **`np.eig()`**: Calcula los autovalores y autovectores de una matriz.
  ```python
  eigenvals, eigenvecs = np.linalg.eig(A)
  ```

---

#### 9. **Matrices Diagonales**
- **`np.diag()`**: Crea una matriz diagonal a partir de una lista o tupla.
  ```python
  diagonal = np.diag([2, 4, 6])
  ```

---

#### 10. **Concatenación de Matrices**
- **`np.vstack()`**: Concatena matrices verticalmente.
  ```python
  vertical = np.vstack((matriz1, matriz2))
  ```

- **`np.hstack()`**: Concatena matrices horizontalmente.
  ```python
  horizontal = np.hstack((matriz1, matriz2))
  ```

---

Con este tutorial, deberías poder realizar operaciones básicas con matrices en Numpy. ¡Practica con ejemplos reales para afianzar tus conocimientos!
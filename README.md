# Repositorio-de-prueba
Repositorio de ejemplo de C++


# Especificación de la Biblioteca para el Tipo String

Esta biblioteca define un conjunto de operaciones sobre el alfabeto $\Sigma$ para la gestión y manipulación de cadenas terminadas en carácter nulo.

---

## 1. Operaciones de Consulta

### IsEmpty
Verifica si una cadena carece de caracteres.
- **Firma:** $isEmpty: \Sigma^* \to \mathbb{B}$
- **Definición:** 
  $$isEmpty(s) = (s = \epsilon)$$

### GetLength
Calcula la cantidad de símbolos en una cadena de forma recursiva.
- **Firma:** $length: \Sigma^* \to \mathbb{N}$
- **Definición:**
  $$length(s) = \begin{cases} 0 & s = \epsilon \\ 1 + length(t) & h \cdot t, h \in \Sigma \end{cases}$$

### AreEqual
Compara si dos cadenas son idénticas en longitud y contenido.
- **Firma:** $areEqual: \Sigma^* \times \Sigma^* \to \mathbb{B}$
- **Definición:**
  $$areEqual(s_1, s_2) = (s_1 = s_2)$$

### IsPalindrome (Función Libre)
Determina si una cadena se lee igual de izquierda a derecha que de derecha a izquierda.
- **Firma:** $isPalindrome: \Sigma^* \to \mathbb{B}$
- **Definición:**
  $$isPalindrome(s) = \begin{cases} true & s = \epsilon \\ \forall i < \lfloor \frac{length(s)}{2} \rfloor : s_i = s_{length(s)-1-i} & s \neq \epsilon \end{cases}$$

---

## 2. Operaciones de Creación o Mutación (Crédito Extra)

### Concatenate
Añade el contenido de una cadena al final de otra.
- **Firma:** $concatenate: \Sigma^* \times \Sigma^* \to \Sigma^*$

### Reverse
Invierte el orden de los caracteres de una cadena.
- **Firma:** $reverse: \Sigma^* \to \Sigma^*$

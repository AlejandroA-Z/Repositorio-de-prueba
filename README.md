### IsPalindrome (Función Libre)
Determina si una cadena se lee igual de izquierda a derecha que de derecha a izquierda.
- **Firma:** $isPalindrome: \Sigma^* \to \mathbb{B}$
- **Definición:**
  $$isPalindrome(s) = \begin{cases} true & s = \epsilon \\ \forall i < \lfloor \frac{length(s)}{2} \rfloor : s_i = s_{length(s)-1-i} & s \neq \epsilon \end{cases}$$

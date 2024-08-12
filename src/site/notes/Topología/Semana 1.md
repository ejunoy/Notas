---
{"dg-publish":true,"permalink":"/topologia/semana-1/"}
---

# 1.11
Todo conjunto de la forma $\{ x:f(x)\geq 0 \}$ es un conjunto nulo:
$$
\{ x: f(x)\geq 0  \} = Z(f \land 0) = Z(f-|f|).
$$
Similarmente,
$$
\{ x :f(x)\leq 0 \} = Z(f \lor 0) = Z(f+|f|).
$$
Entonces, los conjuntos abiertos $$
pos(f) = \{ x:f(x)>0 \}
$$
y $$
neg(f)= \{ x: f(x)<0 \}
$$
son conjuntos conulos, es decir, son complementos de conjuntos nulos.
Reciprocamente, todo conjunto conulo es de la forma $$
X \setminus Z(f) = pos(| f|).
$$
# 1.12
Para una función $f$ en $C(X)$, $f^{-1}$ existe si y sólo si $f$ nunca se hace cero; en otras palabras, $f$ es una unidad de $C(X)$ si y sólo si $Z(f)=\emptyset$.
Similarmente, si $f$ es una unidad de $C^{*}(X)$, entonces $Z(f)= \emptyset$. El recìproco no siempre es cierto, pues el inverso multiplicativo $f^{-1}$ de $f$ en $C(X)$ podría no ser acotado. De hecho, la condición de que $f$ sea una unidad de $C^{*}(X)$ es equivalente a que el cero sea un punto exterior de la imagen de $f$, es decir, que $f$ esté acotada lejos del cero.
# 1.13
*Ejemplos* Un ejemplo familiar e importante de un conjunto compacto es el intervalo cerrado $[0,1]$ es $\mathbb{R}$. Como sabemos $C(\mathbb{R}) =C^{*}(\mathbb{R})$. Como $\mathbb{N}$ es discreto, $C(\mathbb{N})$ coincide con el conjunto de funciones de $\mathbb{N}$ en $\mathbb{R}$, es decir, las suceiones de números reales, también, $C^{*}(\mathbb{N})$ es el conjunto de sucesiones acotadas de números reales.

# 1.14
Para $C' \subseteq C(X)$, escribimos $Z[C']$ para designar a la familia de conjuntos nulos $\{ Z(f): f \in C' \}.$ Por otro lado, la familia $Z[C(X)]$ será denotada por $Z(X)$.
Ya hemos observado que $Z(X)$ es cerrado bajo uniones e intersecciones finitas.

> [!theorem]
> $Z(X)$ es cerrado bajo intersecciones numerables.


`\begin{proof}`
Sea $(f_{n})_{n \in \mathbb{N}}$ una familia de funciones continuas. Para cada $f_{n}$ definimos $g_{n}: X \to \mathbb{R}$ como la funciòn dada por $g_{n}(x) = |f_{n}(x)|\land \frac{1}{2^{n}}$. Nota que para cada $n \in \mathbb{N}$ se tiene que $0\leq g_{n} < \frac{1}{2^{n}}$. De modo que:
$$\begin{align} |\sum_{k=0}^{m} g_{k}(x)-\sum_{k=0}^{n}g_{k}(x)|= |\sum_{k=n+1}^{m} \frac{1}{2^{k}}| \leq \frac{1}{2^{n}} \end{align}$$
Luego, por el criterio de Cauchy, $f := \sum_{k=0}^{\infty } g_{n}$ es una función continua. Además, es claro que $Z(g) = \bigcap_{n \in \mathbb{N}} Z(f_{n})$, de modo que $Z(f)$ es cerrado bajo intersecciones numerables.
`\end{proof}`

Sin embargo, $Z(X)$ no tiene porqué ser cerrado bajo uniones infinitas. De hecho, todo conjunto unitario en $\mathbb{R}$ es un conjunto nulo, sin emabrgo, muchos conjuntos que son uniones infinitas de puntos no son cero conjuntos, inclusive las uniones numerables pueden fallar.
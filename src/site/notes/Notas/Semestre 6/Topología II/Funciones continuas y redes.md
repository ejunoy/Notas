---
{"dg-publish":true,"permalink":"/notas/semestre-6/topologia-ii/funciones-continuas-y-redes/"}
---

> [!theorem|*]
> Sean ${} (X,\tau), (Y,\sigma) {}$ espacios topológicos y sea ${} f: X \to Y {}$ una función. Entonces ${} f {}$ es continua en ${} x_{0} {}$ si y sólo si para cada red ${} (x_{\lambda})_{\lambda \in \mathcal{A}} {}$ que converge a ${} x_{0} {}$ se tiene que ${} (f(x_{\lambda}))_{\lambda \in \mathcal{A}} {}$ converge a ${} f(x_{0}) {}$.
> 

*Demostración.* 
1. ${} \rightarrow {}$ Supongamos que ${} f {}$ es continua en ${} x_{0} {}$. Sea ${} U \in \mathcal{N}(f(x_{0})) {}$. Como ${} f {}$ es continua entonces ${} f^{-1}(U) \in \mathcal{N}(x_{0}) {}$. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red que converge a ${} x_{0} {}$. Entoces existe ${} \lambda_{0} \in \Lambda {}$ tal que si ${} \lambda\geq \lambda_{0} {}$ entonces ${} x_{\lambda} \in f^{-1}(U) {}$, de modo que ${} f(x_{\lambda}) \in U {}$. Por lo tanto ${} (f(x_{\lambda}))_{\lambda \in \Lambda} {}$ converge a ${} f(x_{0}) {}$.
2. Sea ${} A \subseteq X {}$. Sea ${} x_{0} \in \overline{A}{}$. Entonces existe ${} (x_{\lambda})_{\lambda \in \Lambda} \subseteq A {}$ que converge a ${} x_{0} {}$. Entonces ${} (f(x_{\lambda}))_{\lambda \in \Lambda}\subseteq f(A) {}$ converge a ${} f(x_{0}) {}$. Entonces ${} f(x_{0}) \in \overline{f(A)} {}$. Así, ${} f(\overline{A})\subseteq \overline{f(A)} {}$ y ${} f {}$ es continua.
$\blacksquare$
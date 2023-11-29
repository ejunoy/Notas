---
{"dg-publish":true,"permalink":"/notas/semestre-6/topologia-ii/redes-y-compacidad/"}
---

<mark style="background: #FF5582A6;">Recordatorio</mark> 
- ${} \mathcal{C} {}$ tiene la propiedad de la intersección finita (PIF) si para cada ${} \mathcal{F} \subseteq \mathcal{C} {}$ finita se cumple que
$${} \cap  \mathcal{F} \neq  \emptyset . {}$$
- ${} X {}$ es compacto si y sólo si toda familia de subconjuntos cerrados con la PIF tiene intersección no vacía.

> [!theorem|*]
> ${} X {}$ es compacto si y sólo si para cada red ${} (x_{\lambda})_{\lambda\in \Lambda} \subseteq X{}$ existe una subred convergente, lo cual sucede si y sólo si toda red tiene un punto de acumulación.
> 

*Demostración.* 
- ${} \rightarrow {}$ Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red en ${} x {}$. Para cada ${} \lambda \in \Lambda {}$ 
	$${} T_{\lambda }:= \left\{ x_{\mu }: \mu \geq  \lambda    \right\}  . {}$$
	**Observación.** Para cada ${} \lambda_{1},\dots,\lambda_{k} {}$ existe ${} \mu\geq \lambda_{i} {}$ para cada ${} i \in \left\{1,\dots,k \right\} {}$. Entonces ${} x_{\mu} \in T_{\lambda_{i}} \subseteq \overline{T_{\lambda_{i}}} {}$ para cada ${} i \in \left\{1,\dots,k \right\} {}$. Entonces ${} \bigcap_{i=i}^{k}\overline{T_{\lambda_{i}}} \neq \emptyset {}$.
	Entonces ${} \mathcal{C}= \left\{ \overline{T_{\lambda}} \right\}_{\lambda \in \Lambda} {}$ es una familia de subconjuntos cerrados con la PIF.
	Como ${} X {}$ es compacto entonces ${} \bigcap_{\lambda \in \Lambda} \overline{T_{\lambda_{i}} } \neq \emptyset{}$.
	Sea ${} x \in \bigcap_{\lambda \in \Lambda} \overline{T_{\lambda_{i}}} {}$. Entoces para cada ${} U \in \mathcal{N}(x) {}$ y ${} \lambda \in \Lambda {}$, ${} U \cap T_{\lambda} \neq \emptyset {}$. Entonces existe ${} \mu\geq \lambda {}$ tal que ${} x_{\mu} \in U {}$. Entonces ${} x {}$ es un punto de acumulación de ${} (x_{\lambda})_{\lambda\in \Lambda} {}$. Por lo tanto, existe una subred convergente.
- ${} \leftarrow {}$ Supongamos que ${} X {}$ no es compacto. Entonces existe ${} \mathcal{U} {}$ una cubierta abierta de ${} X {}$ sin una subcubierta finita.
	Sea 
	$${} \mathcal{A} = \left\{ \mathcal{V} \subseteq  \mathcal{U} : \left\lvert \mathcal{V} \right\rvert <\infty  \right\}  .{}$$
	Definimos un orden en ${} \mathcal{A} {}$ por ${} \mathcal{V}_{1} \leq \mathcal{V}_{2} \iff \mathcal{V}_{1}\subseteq \mathcal{V}_{2} {}$.
	Como ${} \mathcal{U} {}$ no tiene una subcubierta finita, entonces para cada ${} \mathcal{UV} \in \mathcal{A} {}$ existe ${}x_{\mathcal{V}} \in X \setminus \cup_{V \in \mathcal{V}} V .{}$
	Entonces ${} (x_{\mathcal{U}})_{\mathcal{U} \in \mathcal{A}} {}$ es una red en ${} X {}$. Entonces existe ${} x \in X {}$ un punto de acumulación de la red. Tenemos que existe ${} U \in \mathcal{U} {}$ tal que ${} x \in U {}$, entonces ${} \mathcal{U}_{0}=\left\{ U \right\} \in \mathcal{A} {}$. Entonces existe ${} \mathcal{V} \geq \mathcal{U}_{0} {}$ tal que ${} x_{\mathcal{V}} \in U {}$, pero ${} x_{\mathcal{V}} \in X\setminus \cup_{V \in \mathcal{V}}V \subseteq X\setminus U {}$. Lo cual es imposible.
	${} \therefore X {}$ es compacto.
$\blacksquare$ 



---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/equivalencia-de-compacidad-con-filtros/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*] Equivalencia de compacidad con filtros
> 
> Sea ${} X {}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]]. Son equivalentes:
> 1. ${} X {}$ es compacto.
> 2. Todo [[Conceptos/Semestre 6/Filtro\|filtro]] tiene un punto de acumulación.

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} \mathcal{F} {}$ es compacto. Sea ${} \mathcal{F} {}$ un [[Conceptos/Semestre 6/Filtro\|filtro]]. Considera ${} \mathcal{C}= \left\{ \overline{F}: F \in \mathcal{F} \right\} {}$. Sean ${} \overline{F_{1}}, \dots, \overline{F_{n}} \in \mathcal{C}{}$. Como ${} \mathcal{F} {}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]], entonces
	$${}\emptyset \neq  \bigcap_{i=1} ^{n} F_{i} \in  \mathcal{F}  {}$$
	Entonces 
	$${} \bigcap_{i=1} ^{n}  \overline{F_{i} }  {} \neq  \emptyset .$$
	Entonces ${} \mathcal{C} {}$ tiene la propiedad de la intersección finita y, como ${} X {}$ es compacto, entonces 
	$${} \bigcap_{} \mathcal{C}  \neq \emptyset  .{}$$
	Luego, existe un punto en la cerradura de cada elemento de ${} \mathcal{F} {}$, de modo que éste debe ser un punto de acumulación del [[Conceptos/Semestre 6/Filtro\|filtro]].

- ${} \leftarrow {}$ Sea ${} \mathcal{C} {}$ una familia de conjuntos cerrados con la propiedad de la intersección finita. Sea 
- ${} \leftarrow {}$
	$${} \mathcal{B}=\left\{ \bigcap_{i=1}^{n} C_{i} \vert C_{i} \in  \mathcal{C} , n \in  \mathbb{N}    \right\} .{}$$
	Nota que
	1. ${} \forall B \in \mathcal{B} {}$ se tiene que ${} B \neq \emptyset {}$.
	2. Si ${} B,D \in \mathcal{B} {}$ entonces ${} B \cap D  \in \mathcal{B}{}$.
	Entonces ${} \mathcal{B} {}$ es [[Conceptos/Semestre 6/Base de filtro\|base]] para un [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{F} {}$ en ${} X {}$.
	Por hipótesis ${} \mathcal{F} {}$ tiene un punto de acumulación ${} x {}$ . Es decir,    
	$${} x \in  \bigcap_{F \in \mathcal{F}  }\overline{F} .  {}$$
	Nota que ${} \mathcal{C} \subseteq \mathcal{B} \subseteq \mathcal{F} {}$. Entonces 
	$${} \cap \mathcal{C} \supset \cap \mathcal{F}  {}.$$
	De modo que 
	$${} \bigcap_{C \in  \mathcal{C} } \overline{C}  \supset \bigcap_{F \in \mathcal{F} } \overline{F} . {}$$
	Por lo tanto ${} \cap \mathcal{C} {}$ es no vacío. Entonces ${} X {}$ es compacto.
$\blacksquare$
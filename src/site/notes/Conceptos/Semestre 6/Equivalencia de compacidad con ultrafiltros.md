---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/equivalencia-de-compacidad-con-ultrafiltros/"}
---

#Tema/Topología  #Tipo/Corolario 

> [!corollary|*] Equivalencia de compacidad con ultrafiltros
> 
> ${} X {}$ es compacto si y sólo si todo [[Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] converge.
> 

*Demostración.* 
- ${} \rightarrow {}$ Si ${} \mathcal{G} {}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]], entonces tiene un punto de acumulación. Pero sabemos que los puntos de acumulación de un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] son puntos de convergencia, entonces ${} \mathcal{G} {}$ converge.
- ${} \leftarrow {}$ Sea ${} \mathcal{F} {}$ un [[Conceptos/Semestre 6/Filtro\|filtro]]. Como [[Conceptos/Semestre 6/Todo filtro está contenido en un ultrafiltro\|Todo filtro está contenido en un ultrafiltro]] entonces existe un ultra [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{G} {}$ con ${} \mathcal{F} \subseteq \mathcal{G} {}$. Por hipótesis ${} \mathcal{G} {}$ converge a un punto ${} x {}$. Entonces ${} \mathcal{N}(x)\subseteq \mathcal{G} {}$ y ${} \mathcal{F} \subseteq \mathcal{G} {}$. Entonces para cada ${} U \in \mathcal{N}(x) {}$ y para cada ${} F \in \mathcal{F} {}$ se tiene que ${} U \cap F \in \mathcal{G} {}$ y, por lo tanto, ${} U \cap F \neq \emptyset{}$. Luego, ${} x {}$ es punto de acumulación de ${} \mathcal{F} {}$. Entonces por la [[Conceptos/Semestre 6/Equivalencia de compacidad con filtros\|Equivalencia de compacidad con filtros]] se tiene que ${} X {}$ es compacto. 
$\blacksquare$
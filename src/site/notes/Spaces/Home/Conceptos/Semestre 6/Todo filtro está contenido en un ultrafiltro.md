---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/todo-filtro-esta-contenido-en-un-ultrafiltro/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*] Todo [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] está contenido en un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]
> 
> Sea ${} \mathcal{F} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en un conjunto ${} X {}$. Entonces existe un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] ${} \mathcal{G} {}$ tal que ${} \mathcal{F}\subseteq\mathcal{G} {}$.
> 

*Demostración.* Nota que ${} \left\{\mathcal{G} \vert \mathcal{G} \text{ es filtro en  }X \text{ con } \mathcal{F}\subseteq\mathcal{G} \right\} {}:= \Phi$ es un conjunto parcialmente ordenado. 
Sea ${} \left\{\mathcal{G}_{\alpha} \right\}_{\alpha \in \mathcal{A}} {}$ una cadena no vacía. Sea ${} \mathcal{G}= \bigcup_{\alpha \in \mathcal{A}}\mathcal{G}_{\alpha} {}$. Veamos que ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]].
1. Sea ${} F \in \mathcal{G} {}$ entonces existe ${} \alpha_{0} \in \mathcal{A} {}$ tal que ${} F \in \mathcal{G}_{\alpha_{0}} {}$, entonces ${} F \neq \emptyset {}$.
2. Sean ${} F,G \in \mathcal{G} {}$. Entonces existen ${} \alpha_{1},\alpha_{2} \in \mathcal{A} {}$ tales que ${} F \in \mathcal{G}_{\alpha_{1}} {}$ y ${} G \in \mathcal{G}_{\alpha_{2}} {}$. Como ${} \left\{\mathcal{G}_{\alpha} \right\}_{\alpha \in \mathcal{A}} {}$ es una cadena, entonces ${} F\leq G {}$ o ${} G\leq F {}$, de modo que ${} G \in \mathcal{G}_{\alpha_{1}} {}$ o ${}F \in \mathcal{G}_{\alpha_{2}}  {}$. Entonces ${} G \cap F \in \mathcal{G} {}$.
3. Sea ${} F \in \mathcal{G} {}$ y ${} G \supset F {}$. Entonces existe ${} \alpha_{0} {}$ tal que ${} F \in \mathcal{G}_{\alpha_{0}} {}$. Por lo tanto ${} G \in \mathcal{G}_{\alpha_{0}} {}$ y ${} G \in \mathcal{G} {}$.
Entonces ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] y es cota superior de la cadena ${} \left\{\mathcal{G}_{\alpha} \right\}_{\alpha \in \mathcal{A}} {}$. Entonces toda cadena está acotada superiormente y, por el [[Spaces/Home/Conceptos/Semestre 6/Lema de Zorn\|Lema de Zorn]] se tiene que existe un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \tilde{\mathcal{G}} {}$ maximal con ${} \mathcal{F} \subseteq \tilde{\mathcal{G}}{}$, entonces ${} \tilde{\mathcal{G}} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] que contiene a ${} \mathcal{F} {}$.
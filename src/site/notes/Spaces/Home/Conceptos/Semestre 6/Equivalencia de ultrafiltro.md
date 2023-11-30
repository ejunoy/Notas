---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/equivalencia-de-ultrafiltro/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*] Equivalencia de [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]
> 
> Sea ${} X {}$ un conjunto. Un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] si y sólo si para cada ${} E \subseteq X {}$ se tiene que ${} E \in \mathcal{F} {}$ o ${} X\setminus E  \in \mathcal{F}{}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Sea ${} E\subseteq X {}$ arbitrario   
	- Si existe ${} F \in \mathcal{F}{}$ con ${} F \cap E = \emptyset{}$ entonces ${} F\subseteq X\setminus E {}$, entonces ${} X\setminus E \in \mathcal{F}{}$.
	- Si ${} F \cap E \neq \emptyset {}$ entonces para cada ${} F \in \mathcal{F} {}$ se tiene que ${} E \cap F \neq \emptyset {}$. Sea ${} \mathcal{C}= \left\{ E \cap F\vert F \in \mathcal{F} \right\} {}$.
		- Si ${} E \cap F_{1} {}$, ${} E \cap F_{2} {}$ ${}\in \mathcal{C} {}$  entonces ${} E\cap(F_{1}\cap F_{2}) \subseteq F \in \mathcal{C} {}$.
		Entonces ${} \mathcal{C} {}$ es [[Spaces/Home/Conceptos/Semestre 6/Base de filtro\|base]] para un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]].
		Sea ${} \mathcal{G} {}$ el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} \mathcal{C} {}$. Como ${} E \cap F \subseteq F {}$ entonces ${} F \in \mathcal{G} {}$ y, port lo tanto, ${} \mathcal{F} \subseteq \mathcal{G} {}$ y, como ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]], entonces ${} \mathcal{F}=\mathcal{G} {}$. Ahora, para cda ${} F \in \mathcal{F} {}$ se tiene que ${} F \cap E \subseteq E{}$ entonces ${} E \in \mathcal{F} {}$.
	Así que ${} E \in \mathcal{F} {}$ o ${} x\setminus E \in \mathcal{F}{}$.

- ${} \leftarrow {}$ Supongamos que para cada ${} E \subseteq X {}$ se tiene que ${} E \in \mathcal{F} {}$ o ${} X\setminus E \in \mathcal{F} {}$. Sea ${} \mathcal{G} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] con ${} \mathcal{F}\subseteq \mathcal{G} {}$. Si ${} \mathcal{F} \neq \mathcal{G} {}$, entonces existe ${} G \in \mathcal{G}\setminus \mathcal{F} {}$. Ahora, como ${} G \not \in \mathcal{F} {}$ entonces ${} X\setminus\mathcal{G} \in \mathcal{F} \subseteq \mathcal{G}{}$, de modo que ${} G \cap (X\setminus G) \in \mathcal{G} {}$, lo cual es imposible.
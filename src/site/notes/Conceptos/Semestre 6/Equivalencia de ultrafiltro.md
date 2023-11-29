---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/equivalencia-de-ultrafiltro/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*] Equivalencia de [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]]
> 
> Sea ${} X {}$ un conjunto. Un [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{F} {}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] si y sólo si para cada ${} E \subseteq X {}$ se tiene que ${} E \in \mathcal{F} {}$ o ${} X\setminus E  \in \mathcal{F}{}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} \mathcal{F} {}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]]. Sea ${} E\subseteq X {}$ arbitrario   
	- Si existe ${} F \in \mathcal{F}{}$ con ${} F \cap E = \emptyset{}$ entonces ${} F\subseteq X\setminus E {}$, entonces ${} X\setminus E \in \mathcal{F}{}$.
	- Si ${} F \cap E \neq \emptyset {}$ entonces para cada ${} F \in \mathcal{F} {}$ se tiene que ${} E \cap F \neq \emptyset {}$. Sea ${} \mathcal{C}= \left\{ E \cap F\vert F \in \mathcal{F} \right\} {}$.
		- Si ${} E \cap F_{1} {}$, ${} E \cap F_{2} {}$ ${}\in \mathcal{C} {}$  entonces ${} E\cap(F_{1}\cap F_{2}) \subseteq F \in \mathcal{C} {}$.
		Entonces ${} \mathcal{C} {}$ es base para un [[Conceptos/Semestre 6/Filtro\|filtro]].
		Sea ${} \mathcal{G} {}$ el [[Conceptos/Semestre 6/Filtro\|filtro]] generado por ${} \mathcal{C} {}$. Como ${} E \cap F \subseteq F {}$ entonces ${} F \in \mathcal{G} {}$ y, port lo tanto, ${} \mathcal{F} \subseteq \mathcal{G} {}$ y, como ${} \mathcal{F} {}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]], entonces ${} \mathcal{F}=\mathcal{G} {}$. Ahora, para cda ${} F \in \mathcal{F} {}$ se tiene que ${} F \cap E \subseteq E{}$ entonces ${} E \in \mathcal{F} {}$.
	Así que ${} E \in \mathcal{F} {}$ o ${} x\setminus E \in \mathcal{F}{}$.

- ${} \leftarrow {}$ Supongamos que para cada ${} E \subseteq X {}$ se tiene que ${} E \in \mathcal{F} {}$ o ${} X\setminus E \in \mathcal{F} {}$. Sea ${} \mathcal{G} {}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] con ${} \mathcal{F}\subseteq \mathcal{G} {}$. Si ${} \mathcal{F} \neq \mathcal{G} {}$, entonces existe ${} G \in \mathcal{G}\setminus \mathcal{F} {}$. Ahora, como ${} G \not \in \mathcal{F} {}$ entonces ${} X\setminus\mathcal{G} \in \mathcal{F} \subseteq \mathcal{G}{}$, de modo que ${} G \cap (X\setminus G) \in \mathcal{G} {}$, lo cual es imposible.
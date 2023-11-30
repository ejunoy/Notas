---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/cerradura-con-filtros/"}
---

#Enconstrucción
#Tema/Topología  #Tipo/Teorema  
> [!theorem|*] Cerradura con filtros
> Sea ${}(X,\tau){}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]]. ${}A\subseteq X{}$. Entonces un punto ${}x{}$ está en ${}\overline{ A}{}$ si y solo si existe un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${}\mathcal{F}{}$ tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{F} \to x{}$.

*Demostración.* 
- ${}\rightarrow{}$ Sea ${}x \in \overline{A}{}$. Sea ${}\mathcal{C}= \left\{ U \cap A : U \in \mathcal{N}(x) \right\}{}$. Entonces ${}\mathcal{C}{}$ es [[Spaces/Home/Conceptos/Semestre 6/Base de filtro\|base]] para un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${}\mathcal{F}= \mathcal{F}_{\mathcal{C}}{}$. Además, se cumple que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x)\subseteq \mathcal{F}{}$.
- ${}\leftarrow{}$ Supongamos que ${}\mathcal{F}{}$ es un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x) \subseteq \mathcal{F}{}$. Entonces para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}U \cap A \in \mathcal{F}{}$, de modo que ${}U \cap A \neq \emptyset{}$ y ${}x \in \overline{A}{}$.
$\blacksquare$